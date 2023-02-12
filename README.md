 
<h1 align="center">    
    Welcome to #70DaysOfServiceMesh!!!    
</h1>

![Banner](https://user-images.githubusercontent.com/91419219/213897837-857e8855-0203-4462-8379-9a712843246b.png)

 
### Welcome to #70DaysOfServiceMesh!!!
Inspired by Michael Cades' #90DaysOfDevOps and his ask for me to participate in his 2023 iteration to discuss 7 Days of Service Mesh, I decided to create a #70DaysOfServiceMesh.

70 Days of Service Mesh allows me to dig into plenty of areas to help myself (and others) better understand the inner workings of a service mesh. Some days will be a bit of a mini blogpost while other days might be very tutorial oriented.

Also, these are 70 sequential days of service mesh. It means I'll spend about day focusing on one topic. Hopefully I wrap this up within 90 days because 2023 is starting to look BUSY.

I'll add contribution guidelines in the future!

In this repo, we'll dig into a structured and iterative approach to learning Service Mesh.

### The topics covered in this repository:
- What is a Service Mesh
- Comparison of Service Meshes
- Networking Recap
- Kubernetes Recap
- Envoy
- Traffic Engineering
- Application Resiliency
- Observability
- Security and AuthN/AuthZ
- Istio Ambient Mesh
- Expanded areas of Istio

### The table below outlines what we'll cover in 70 Days of Service Mesh, with Istio being the main focus.

**Note** Some of this is subject to change.

| Day | Topic | Content | Description |
---|---|---|---|
0 | The Setup | Informational | Setting up this repo
1 | Let's break down a Service Mesh | Informational | An introduction to Service Mesh, the use-cases, and the problems it aims to solve.
2 | Install and Test a Service Mesh | Tutorial | Let's install our first service mesh
3 | Comparing Different Service Meshes | Informational | A comparison of Istio, Linkerd, Consul, AWS App Mesh and Cilium
4 | Traffic Engineering Basics | Tutorial | Let's test out traffic routing, and shifting
5 | Observability in your Mesh | Tutorial | Let's see what's going on in our mesh
6 | Securing your microservices | Tutorial | Let's secure our microservices
7 | Resilient Microservices | Tutorial | Let's build some resilient microservices
8 | Setting up a Kubernetes environment for Service Mesh | Tutorial | Prequisites and requirements for a Service Mesh Playground
9 | Recap: TCP/IP and DNS | Informational | What is TCP/IP and how does this relate to DNS?
10 | Recap: Kubernetes Networking and DNS | Tutorial | Let's dive into Kubernetes Networking and DNS
11 | Recap: Kubernetes Services | Tutorial | How do we connect to services within our cluster?
12 | Ingress Resource | Tutorial | Let's explore how we get traffic into our cluster.
13 | Gateway API in Kubernetes | Tutorial | This is a new Ingress spec that allows for granular control of ingress routing
14 | Diving into the Envoy Proxy | Informational | Let's investigate this highly power L4/L7 proxy
15 | Interacting with Envoy | Tutorial | Let's interact with Envoy and understand it's power
16 | Istio Architecture and Components | Informational | Time to review the Istio Service Mesh and it's architecture
17 | Istio installation methods | Informational | We will review the various installation methods, and profiles.
18 | Install Istio and the Demo Profile | Tutorial | Let's install service mesh on our cluster.
19 | The Virtual Service, Destination Rule, and Service Entry CRDs | Informational | Breaking down traffic routing resources.
20 | Istio Ingress Gateway | Tutorial | Let's dive into the Istio Ingress Gateway and configure it.
21 | The Istio Sidecar and Sidecar Injection | Tutorial | Understanding how Envoy plays the role of Sidecar and what the sidecar does in the service Mesh
22 | Traffic Engineering - Releases | Informational | Understading Dark Launches, Canaries and release practices
23 | Traffic Engineering - Request Routing | Tutorial | Understanding how to route requests and shift traffic based on various conditons
24 | Traffic Engineering - Traffic Shift | Tutorial | How to shift traffic based on various conditons
25 | Traffic Engineering - Traffic Mirroring | Tutorial | Understanding how traffic mirroring can help with releases.
26 | Microservices Resiliency Expanded | Informational | Client-side LB, Locality-aware LB, Timeouts and retries, circuit breaking
27 | Resiliency - Client-side Load-balancing | Tutorial | Testing out resiliency with Client-side Load-balancing
28 | Resiliency - Locality-aware Load-balancing | Tutorial | Testing out resiliency with Locality
29 | Resiliency - Retries and Timeouts | Tutorial | Testing out resiliency with Retries and Timeouts
30 | Resiliency - Circuit Breaking | Tutorial | Testing out resiliency with Circuit Breaking
31 | The Four Golden Signals - Latency, Errors, Traffic, Saturation | Informational | Diving into Latency, Errors, Traffic and Saturation
32 | Observability in your Mesh - Expanded | Informational | Understanding traffic patterns and using the Mesh to gives our observability
33 | Istio Control and Data Plane Metrics | Tutorial | Gathering information from various Istio components to understand behavior
34 | Using Prometheus and Grafana to scrape Istio Metrics  | Tutorial | Scraping metrics with Prometheus and Grafana
35 | Distributed Tracing in Istio with Jaegar Part 1 | Tutorial | Let's get familiar with Distributed tracing and Jaegar
36 | Distributed Tracing in Istio with Jaegar Part 2 | Tutorial | Let's use  Jaegar to understand a request flow
37 | Visualization with Kiali | Tutorial | Using Kiali, let's visualize microservices interactions.
38 | Understanding certificates and TLS and mTLS | Informational | What are Certificates and what are TLS and mTLS?
39 | Understanding JWT | Informational | How does JSON Web Tokens work and provide an authentication mechanism?
40 | SPIFFE Identity | Informational | Understanding SPIFFE ID and how it relates to Istio
41 | Securing your microservices - Expanded | Informational | Let's secure our microservices and understand the need behind this.
42 | Secured Microservices - mTLS and Peer-AuthN | Tutorial | Mutual TLS and Peer Authentication in Istio
43 | Secured Microservices - Service-to-Service AuthZ Part 1 | Tutorial | Understanding the setup for for AuthZ
44 | Secured Microservices - Service-to-Service AuthZ Part 2 | Tutorial | Testing out AuthZ
45 | Secured Microservices - End-user Client Authentication  | Tutorial | Testing out Auth with JWT
46 | Secured Microservices - ExtAuthZ  | Tutorial | Setting up ExtAuthZ
47 | Troubleshooting: The Istio Data Plane Part 1 | Tutorial | Troubleshooting: The Istio Data Plane
48 | Troubleshooting: The Istio Data Plane Part 2 | Tutorial | Troubleshooting: The Istio Data Plane
49 | Troubleshooting: The Istio Control Plane Part 1| Tutorial | Troubleshooting: The Istio Control Plane
50 | Troubleshooting: The Istio Control Plane Part 2 | Tutorial | Troubleshooting: The Istio Control Plane
51 | Scaling the Istio Service Mesh - Multi-cluster Service Mesh | Informational | Understanding the need for Multiple Clusters running Service Mesh, a quick peak at multi-cluster offerings (Gloo Mesh, Anthos Service Mesh, Tanzu Service Mesh)
52 | Scaling the Istio Service Mesh - Multi-cluster Service Mesh | Tutorial | Scaling the Istio Service Mesh
53 | Scaling the Istio Service Mesh - Multi-cluster Service Mesh | Tutorial | Scaling the Istio Service Mesh
54 | Virtual Machines in your Service Mesh | Informational | How do we connect VMs to the Mesh?
55 | Virtual Machines in your Service Mesh | Tutorial | How do we connect VMs to the Mesh?
56 | Istio and WebAssembly | Informational | Istio and extending the data path for WebAssembly
57 | Istio and Cert Manager | Informational | Why use Cert-manager with Istio?
58 | Istio and Inlets | Tutorial | Using Inlets for the LoadBalancer Service for Istio Ingress Gateways
59 | The Istio-CNI | Informational | Using the Istio-CNI to reroute traffic for side-car operations
60 | Sidecars vs Sidecar-less | Informational | Understanding a world where Sidecar and Sidecar-less coexist.
61 | Istio Ambient Mesh - Sidecar-less Service Mesh | Informational | Sidecar-less Service Mesh
62 | Istio Ambient Mesh - Architecture | Informational | Sidecar-less Service Mesh Architecture
63 | Istio Ambient Mesh - Installation | Tutorial | Installing Istio in Ambient Mode
64 | Istio Ambient Mesh - ztunnel | Tutorial | Breaking down ztunnel
65 | Istio Ambient Mesh - Waypoint Proxy | Tutorial | Using the Waypoint Proxy
66 | Istio Ambient Mesh - Testing out sidecar-less | Tutorial | Sidecar-less operations
67 | Istio Ambient Mesh - Sidecar and Sidecar-less together | Tutorial | The best of both worlds in Service Mesh
68 | A Rust-based proxy with Istio Ambient Mesh | Informational | The reasoning behind a rust-based proxy.
69 | Contributing to the Istio Project | Informational | How do we contribute to the Istio project?
70 | Additional Resources and Playgrounds | Informational | MORE INFO =D

### Thanks to the all Contributors ❤️

<img src="https://contrib.rocks/image?repo=distributethe6ix/70DaysOfServiceMesh" />
