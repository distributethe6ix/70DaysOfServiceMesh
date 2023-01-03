# 70DaysOfServiceMesh

## Welcome to #70DaysOfServiceMesh!!!

In this repo, we'll dig into a structured and iterative approach to learning Service Mesh.

The topics covered in this repository:
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

The table below outlines what we'll cover in 70 Days of Service Mesh, with Istio being the main focus.
| Day | Topic | Content | Description |
---|---|---|---|
0 | The Setup | Informational | Setting up this repo
1 | Let's break down a Service Mesh | Informational | An introduction to Service Mesh, the use-cases, and the problems it aims to solve.
2 | Comparing Different Service Meshes | Informational | A comparison of Istio, Linkerd, Consul, AWS App Mesh and Cilium
3 | Install and Test a Service Mesh | Tutorial | Let's install our first service mesh using some scripts.
4 | Traffic Engineering Basics | Tutorial | Let's test out traffic routing, and shifting
5 | Observability in your Mesh | Tutorial | Let's see what's going on in our mesh
6 | Securing your microservices | Tutorial | Let's secure our microservices
7 | Resilient Microservices | Tutorial | Let's build some resilient microservices
8 | Setting up a Kubernetes environment for Service Mesh | Tutorial | Prequisites and requirements for a Service Mesh Playground
9 | Recap: IP |  TCP |  and DNS | Informational | What is TCP/IP and how does this relate to DNS?
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
32 | Observability in your Mesh - Expanded | Informational | 
33 | Istio Control and Data Plane Metrics | Tutorial | 
34 | Using Prometheus and Grafana to scrape Istio Metrics  | Tutorial | 
35 | Distributed Tracing in Istio with Jaegar | Tutorial | 
36 | Distributed Tracing in Istio with Jaegar | Tutorial | 
37 | Visualization with Kiali | Tutorial | 
38 | Understanding certificates and TLS and mTLS | Informational | 
39 | Understanding JWT | Informational | 
40 | SPIFFE Identity | Informational | 
41 | Securing your microservices - Expanded | Informational | 
42 | Secured Microservices - mTLS and Peer-AuthN | Tutorial | 
43 | Secured Microservices - Service-to-Service AuthZ | Tutorial | 
44 | Secured Microservices - Service-to-Service AuthZ | Tutorial | 
45 | Secured Microservices - End-user Client Authentication  | Tutorial | 
46 | Secured Microservices - ExtAuthZ  | Tutorial | 
47 | Troubleshooting: The Istio Data Plane | Tutorial | 
48 | Troubleshooting: The Istio Data Plane | Tutorial | 
49 | Troubleshooting: The Istio Control Plane | Tutorial | 
50 | Troubleshooting: The Istio Control Plane | Tutorial | 
51 | Scaling the Istio Service Mesh - Multi-cluster Service Mesh | Informational | 
52 | Scaling the Istio Service Mesh - Multi-cluster Service Mesh | Tutorial | 
53 | Scaling the Istio Service Mesh - Multi-cluster Service Mesh | Tutorial | 
54 | Virtual Machines in your Service Mesh | Informational | 
55 | Virtual Machines in your Service Mesh | Tutorial | 
56 | Istio and WebAssembly | Informational | 
57 | Istio and Cert Manager | Informational | 
58 | Istio and Inlets | Tutorial | 
59 | The Istio-CNI | Informational | 
60 | Sidecars vs Sidecar-less | Informational | 
61 | Istio Ambient Mesh - Sidecar-less Service Mesh | Informational | 
62 | Istio Ambient Mesh - Architecture | Informational | 
63 | Istio Ambient Mesh - Installation | Tutorial | 
64 | Istio Ambient Mesh - ztunnel | Tutorial | 
65 | Istio Ambient Mesh - Waypoint Proxy | Tutorial | 
66 | Istio Ambient Mesh - Testing out sidecar-less | Tutorial | 
67 | Istio Ambient Mesh - Sidecar and Sidecar-less together | Tutorial | 
68 | A Rust-based proxy with Istio Ambient Mesh | Informational | 
69 | Contributing to the Istio Project | Informational | 
70 | Additional Resources and Playgrounds | Informational | 
