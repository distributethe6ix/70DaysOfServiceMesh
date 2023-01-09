## 4 - Traffic Engineering Basics
> **Tutorial**
> *Let's test out traffic routing, and shifting*

### Reviewing Key Traffic Management Concepts
Welcome to Day 4 :smile:!!!

In future days of #70DaysofServiceMesh, we'll dig into specific traffic routing resources and how their used. I'm going to review some of these concepts very briefly and come back and revisit these in detail. 

Traffic management is an important topics in the world of microservices communication because, you have not one or two, but thousands of services making requests to each other. In the world of physical networking, network devices can be used for flow control and packet routing, but because the size of our networks have grown to accomodate microservices communications; manually creating the path way for each to connect does not scale well. 

Kubernetes has done quite a lot to simplify networking for microservices through technologies like CNI, Ingress (and more recently), Gateway API. There are other challenges around traffic routing that can be solved with custom-tailored solutions.

Some of the key areas to address with traffic management are:
- Request Routing
- Traffic Splitting
- Traffic Shifting
- Releasing (new versions of your app)
- Traffic mirroring
- Load-balancing

Traffic, or requests, will always enter the Service Mesh through some Ingress, such as the Istio-Ingress-Gateway. Once in the mesh, the request might need to make its way through multiple services before a final response is formed. Each of the microservices, will have a sidecar to process the request and return some response. But, we also need to know how each of these services gets to other services, and what to do when these inbound requests come in.

Client ---> Bookinfo ----> | ProductPage ---> Reviews ---> Ratings |

In the flow above, the client makes a request to Bookinfo (via a DNS name) which is then translated into request towards the first service in the path, ProductPage, which then needs to illicit a respect from Reviews, and Reviews from Ratings. 

Let's explore the components that make this happen, briefly, and revisit these in the future.

#### Istio Ingress Gateway
As mentioned previously, the Istio Ingress Gateway is the entrypoint for requests getting into the mesh. The Istio Ingress Gateway is a resource deployed with both a Deployment and Service defined with a Load Balancer. This is advantageous, because you can create an Istio Ingress resource that listens on certain ports (HTTP) for request to hostnames like istio.io. And you can do this for multiple hosts. This is important because you can virtually overload the resource by creating multiple Ingress resources for the same gateway. This saves you on procuring multiple load-balancers per service.

Interestingly enough, any service you expose with the Istio Ingress Gateway, means that its service type will be set to ClusterIP. We don't connect to the service directly, we do so via the Ingress Gateway. This is also a layer of security with TLS.

You configure an Istio Ingress Gateway resource, and then an associated Virtual Service to route to your services

Istio's Ingress Gateway uses the Proxyv2 image which is purpose-built Envoy proxy, for Istio.

#### Sidecars
Sidecars are an important traffic management tool as they live right alongside each microservice and will proxy requests on behalf of them. 
The sidecars behave in the same manner as the Istio Ingress Gateway, and will receive and process requests, and provide responses appropriately (as they are configured to). The sidecars also play a huge role with observability and security, which I'll explore later.

Istio's sidecar uses the Proxyv2 image which is purpose-built Envoy proxy, for Istio.

#### Virtual Services

#### Destination Rules
These tell us what to do with the request.

#### Service Entries
I'll dive into this later, but Service Entries provide a mechanism for internal services to know how to route to external services, like a Database, or Git repo, or Object storage, for example. This can all be controlled using Service Entries. 

This can be used to control outbound requests as well, but requires a bit of control plane rework. More on this on later.

### Setting up Request Routing

### Setting up Traffic Shifting
So Let's begin