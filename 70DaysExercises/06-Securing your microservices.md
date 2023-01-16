## 6 - Securing your microservices
> **Tutorial**
>> *Let's secure our microservices*

Security is an extensive area when in comes to microservices. I could basically spend an entire 70days on just security alone but, I want to get to the specifics of testing this out in a lab environment with a Service Mesh.

Before I do, what security concerns am I addressing with a Service Mesh?
- Identity
- Policy
- Authorization
- Authentication
- Encrpytion
- Data Loss Prevention.

There's plenty to dig into with these but what specifically of Service Mesh helps us acheive these?

The sidecar, an ingress gateway, a node-level proxy, and the service mesh control plane interacting with the Kubernetes layer.

As a security operator, I may issue policy configurations, or authentication configurations to the Istio control plane which in turn provides this to the Kubernetes API to turn these into runtime configurations for pods and other resources. 

In Kubernetes, the CNI layer may be able to provide a limited amount of network policy and encryption. Looking at a service mesh, encryption can be provided through mutual-TLS, or mTLS for service-to-service communication, and this same layer can provide a mechanism for Authentication using strong identities in SPIFFE ID format. Layer 7 Authorization is another capability of a service mesh. We can authorize certain services to perform actions (HTTP operations) against other services. 

Let's review what Istio offers and proceed to configure some of this. We will explore some of these in greater detail in future days.

### Istio Peer Authentication and mTLS

### Configuring Istio Peer AuthN and Strict mTLS

### Istio Layer 7 Authorization 

### Configuring L7 Authorization Policies



