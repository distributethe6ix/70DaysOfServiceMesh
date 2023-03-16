 # 70DaysOfServiceMesh
 <h1 align="center">    
 <img src="./banner.png" /> 
 <br>
<a href="https://github.com/distributethe6ix/70DaysOfServiceMesh/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/distributethe6ix/70DaysOfServiceMesh"></a>
<a href="https://github.com/distributethe6ix/70DaysOfServiceMesh/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/distributethe6ix/70DaysOfServiceMesh"></a>
<a href="https://github.com/distributethe6ix/70DaysOfServiceMesh/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/distributethe6ix/70DaysOfServiceMesh"></a>
<a href="https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/distributethe6ix/70DaysOfServiceMesh"></a> 

</h1>

## Welcome to #70DaysOfServiceMesh!!!
Inspired by Michael Cades' #90DaysOfDevOps and his ask for me to participate in his 2023 iteration to discuss 7 Days of Service Mesh, I decided to create a #70DaysOfServiceMesh.

70 Days of Service Mesh allows me to dig into plenty of areas to help myself (and others) better understand the inner workings of a service mesh. Some days will be a bit of a mini blogpost while other days might be very tutorial oriented.

Also, these are 70 sequential days of service mesh. It means I'll spend about day focusing on one topic. Hopefully I wrap this up within 90 days because 2023 is starting to look BUSY.

In this repo, we'll dig into a structured and iterative approach to learning Service Mesh.

## The topics covered in this repository:
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
1 | [Let's break down a Service Mesh](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/01-Let's%20break%20down%20a%20Service%20Mesh.md) | Informational | An introduction to Service Mesh, the use-cases, and the problems it aims to solve.
2 | [Install and Test a Service Mesh](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/02-Install%20and%20Test%20a%20Service%20Mesh.md) | Tutorial | Let's install our first service mesh
3 | [Comparing Different Service Meshes](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/03-Comparing%20Different%20Service%20Meshes.md) | Informational | A comparison of Istio, Linkerd, Consul, AWS App Mesh and Cilium
4 | [Traffic Engineering Basics](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/04-Traffic%20Engineering%20Basics.m) | Tutorial | Let's test out traffic routing, and shifting
5 | [Observability in your Mesh](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/05-Observability%20in%20your%20Mesh.md) | Tutorial | Let's see what's going on in our mesh
6 | [Securing your microservices](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/06-Securing%20your%20microservices.md) | Tutorial | Let's secure our microservices
7 | [Resilient Microservices](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/07-Resilient%20Microservices.md) | Tutorial | Let's build some resilient microservices
8 | [Setting up a Kubernetes environment for Service Mesh](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/08-Setting%20up%20a%20Kubernetes%20environment%20for%20Service%20Mesh.md) | Tutorial | Prequisites and requirements for a Service Mesh Playground
9 | [Recap: TCP/IP and DNS](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/09-Recap:%20TCPIP%20and%20DNS.md) | Informational | What is TCP/IP and how does this relate to DNS?
10 | [Recap: Kubernetes Networking and DNS](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/10-Recap:%20Kubernetes%20Networking%20and%20DNS.md) | Tutorial | Let's dive into Kubernetes Networking and DNS
11 | [Recap: Kubernetes Services](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/11-Recap:%20Kubernetes%20Services.md) | Tutorial | How do we connect to services within our cluster?
12 | [Ingress Resource](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/12-Ingress%20Resource.md)| Tutorial | Let's explore how we get traffic into our cluster.
13 | [Gateway API in Kubernetes](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/13-Gateway%20API%20in%20Kubernetes.md) | Tutorial | This is a new Ingress spec that allows for granular control of ingress routing
14 | [Diving into the Envoy Proxy](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/14-Diving%20into%20the%20Envoy%20Proxy.md) | Informational | Let's investigate this highly power L4/L7 proxy
15 | [Interacting with Envoy](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/15-Interacting%20with%20Envoy.md) | Tutorial | Let's interact with Envoy and understand it's power
16 | [Istio Architecture and Components](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/16-Istio%20Architecture%20and%20Components.md) | Informational | Time to review the Istio Service Mesh and it's architecture
17 | [Istio installation methods](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/17-Istio%20installation%20methods.md) | Informational | We will review the various installation methods, and profiles.
18 | [Install Istio and the Demo Profile](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/18-Install%20Istio%20and%20the%20Demo%20Profile.md) | Tutorial | Let's install service mesh on our cluster.
19 | [The Virtual Service, Destination Rule, and Service Entry CRDs](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/19-The%20Virtual%20Service%2C%20Destination%20Rule%2C%20and%20Service%20Entry%20CRDs.md) | Informational | Breaking down traffic routing resources.
20 | [Istio Ingress Gateway](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/20-Istio%20Ingress%20Gateway.md) | Tutorial | Let's dive into the Istio Ingress Gateway and configure it.
21 | [The Istio Sidecar and Sidecar Injection](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/21-The%20Istio%20Sidecar%20and%20Sidecar%20Injection.md) | Tutorial | Understanding how Envoy plays the role of Sidecar and what the sidecar does in the service Mesh
22 | [Traffic Engineering - Releases](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/22-Traffic%20Engineering%20-%20Releases.md) | Informational | Understading Dark Launches, Canaries and release practices
23 | [Traffic Engineering - Request Routing](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/23-Traffic%20Engineering%20-%20Request%20Routing.md) | Tutorial | Understanding how to route requests and shift traffic based on various conditons
24 | [Traffic Engineering - Traffic Shift](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/24-Traffic%20Engineering%20-%20Traffic%20Shift.md) | Tutorial | How to shift traffic based on various conditons
25 | [Traffic Engineering - Traffic Mirroring](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/25-Traffic%20Engineering%20-%20Traffic%20Mirroring.md) | Tutorial | Understanding how traffic mirroring can help with releases.
26 | [Microservices Resiliency Expanded](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/26-Microservices%20Resiliency%20Expanded.md) | Informational | Client-side LB, Locality-aware LB, Timeouts and retries, circuit breaking
27 | [Resiliency - Client-side Load-balancing](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/27-Resiliency%20-%20Client-side%20Load-balancing.md) | Tutorial | Testing out resiliency with Client-side Load-balancing
28 | [Resiliency - Locality-aware Load-balancing](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/28-Resiliency%20-%20Locality-aware%20Load-balancing.md) | Tutorial | Testing out resiliency with Locality
29 | [Resiliency - Retries and Timeouts](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/29-Resiliency%20-%20Retries%20and%20Timeouts.md) | Tutorial | Testing out resiliency with Retries and Timeouts
30 | [Resiliency - Circuit Breaking](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/30-Resiliency%20-%20Circuit%20Breaking.md) | Tutorial | Testing out resiliency with Circuit Breaking
31 | [The Four Golden Signals - Latency, Errors, Traffic, Saturation](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/31-The%20Four%20Golden%20Signals%20-%20Latency%2C%20Errors%2C%20Traffic%2C%20Saturation.md) | Informational | Diving into Latency, Errors, Traffic and Saturation
32 | [Observability in your Mesh - Expanded](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/32-Observability%20in%20your%20Mesh%20-%20Expanded.md) | Informational | Understanding traffic patterns and using the Mesh to gives our observability
33 | [Istio Control and Data Plane Metrics](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/33-Istio%20Control%20and%20Data%20Plane%20Metrics.md) | Tutorial | Gathering information from various Istio components to understand behavior
34 | [Using Prometheus and Grafana to scrape Istio Metrics](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/34-Using%20Prometheus%20and%20Grafana%20to%20scrape%20Istio%20Metrics%20.md)  | Tutorial | Scraping metrics with Prometheus and Grafana
35 | [Distributed Tracing in Istio with Jaegar Part 1](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/35-Distributed%20Tracing%20in%20Istio%20with%20Jaegar.md) | Tutorial | Let's get familiar with Distributed tracing and Jaegar
36 | [Distributed Tracing in Istio with Jaegar Part 2](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/36-Distributed%20Tracing%20in%20Istio%20with%20Jaegar.md) | Tutorial | Let's use  Jaegar to understand a request flow
37 | [Visualization with Kiali](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/37-Visualization%20with%20Kiali.md) | Tutorial | Using Kiali, let's visualize microservices interactions.
38 | [Understanding certificates and TLS and mTLS](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/38-Understanding%20certificates%20and%20TLS%20and%20mTLS.md) | Informational | What are Certificates and what are TLS and mTLS?
39 | [Understanding JWT](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/39-Understanding%20JWT.md) | Informational | How does JSON Web Tokens work and provide an authentication mechanism?
40 | [SPIFFE Identity](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/40-SPIFFE%20Identity.md) | Informational | Understanding SPIFFE ID and how it relates to Istio
41 | [Securing your microservices - Expanded](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/41-Securing%20your%20microservices%20-%20Expanded.md) | Informational | Let's secure our microservices and understand the need behind this.
42 | [Secured Microservices - mTLS and Peer-AuthN](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/42-Secured%20Microservices%20-%20mTLS%20and%20Peer-AuthN.md) | Tutorial | Mutual TLS and Peer Authentication in Istio
43 | [Secured Microservices - Service-to-Service AuthZ Part 1](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/43-Secured%20Microservices%20-%20Service-to-Service%20AuthZ.md) | Tutorial | Understanding the setup for for AuthZ
44 | [Secured Microservices - Service-to-Service AuthZ Part 2](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/44-Secured%20Microservices%20-%20Service-to-Service%20AuthZ.md) | Tutorial | Testing out AuthZ
45 | [Secured Microservices - End-user Client Authentication](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/45-Secured%20Microservices%20-%20End-user%20Client%20Authentication%20.md)  | Tutorial | Testing out Auth with JWT
46 | [Secured Microservices - ExtAuthZ](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/46-Secured%20Microservices%20-%20ExtAuthZ%20.md)  | Tutorial | Setting up ExtAuthZ
47 | [Troubleshooting: The Istio Data Plane Part 1](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/47-Troubleshooting:%20The%20Istio%20Data%20Plane.md) | Tutorial | Troubleshooting: The Istio Data Plane
48 | [Troubleshooting: The Istio Data Plane Part 2](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/48-Troubleshooting:%20The%20Istio%20Data%20Plane.md) | Tutorial | Troubleshooting: The Istio Data Plane
49 | [Troubleshooting: The Istio Control Plane Part 1](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/49-Troubleshooting:%20The%20Istio%20Control%20Plane.md)| Tutorial | Troubleshooting: The Istio Control Plane
50 | [Troubleshooting: The Istio Control Plane Part 2](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/50-Troubleshooting:%20The%20Istio%20Control%20Plane.md) | Tutorial | Troubleshooting: The Istio Control Plane
51 | [Scaling the Istio Service Mesh - Multi-cluster Service Mesh](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/51-Scaling%20the%20Istio%20Service%20Mesh%20-%20Multi-cluster%20Service%20Mesh.md) | Informational | Understanding the need for Multiple Clusters running Service Mesh, a quick peak at multi-cluster offerings (Gloo Mesh, Anthos Service Mesh, Tanzu Service Mesh)
52 | [Scaling the Istio Service Mesh - Multi-cluster Service Mesh](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/52-Scaling%20the%20Istio%20Service%20Mesh%20-%20Multi-cluster%20Service%20Mesh.md) | Tutorial | Scaling the Istio Service Mesh
53 | [Scaling the Istio Service Mesh - Multi-cluster Service Mesh](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/53-Scaling%20the%20Istio%20Service%20Mesh%20-%20Multi-cluster%20Service%20Mesh.md) | Tutorial | Scaling the Istio Service Mesh
54 | [Virtual Machines in your Service Mesh](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/54-Virtual%20Machines%20in%20your%20Service%20Mesh.md) | Informational | How do we connect VMs to the Mesh?
55 | [Virtual Machines in your Service Mesh](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/55-Virtual%20Machines%20in%20your%20Service%20Mesh.md) | Tutorial | How do we connect VMs to the Mesh?
56 | [Istio and WebAssembly](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/56-Istio%20and%20WebAssembly.md) | Informational | Istio and extending the data path for WebAssembly
57 | [Istio and Cert Manager](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/57-Istio%20and%20Cert%20Manager.md) | Informational | Why use Cert-manager with Istio?
58 | [Istio and Inlets](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/58-Istio%20and%20Inlets.md) | Tutorial | Using Inlets for the LoadBalancer Service for Istio Ingress Gateways
59 | [The Istio-CNI](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/59-The%20Istio-CNI.md) | Informational | Using the Istio-CNI to reroute traffic for side-car operations
60 | [Sidecars vs Sidecar-less](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/60-Sidecars%20vs%20Sidecar-less.md) | Informational | Understanding a world where Sidecar and Sidecar-less coexist.
61 | [Istio Ambient Mesh - Sidecar-less Service Mesh](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/61-Istio%20Ambient%20Mesh%20-%20Sidecar-less%20Service%20Mesh.md) | Informational | Sidecar-less Service Mesh
62 | [Istio Ambient Mesh - Architecture](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/62-Istio%20Ambient%20Mesh%20-%20Architecture.md) | Informational | Sidecar-less Service Mesh Architecture
63 | [Istio Ambient Mesh - Installation](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/63-Istio%20Ambient%20Mesh%20-%20Installation.md) | Tutorial | Installing Istio in Ambient Mode
64 | [Istio Ambient Mesh - ztunnel](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/64-Istio%20Ambient%20Mesh%20-%20ztunnel.md) | Tutorial | Breaking down ztunnel
65 | [Istio Ambient Mesh - Waypoint Proxy](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/65-Istio%20Ambient%20Mesh%20-%20Waypoint%20Proxy.md) | Tutorial | Using the Waypoint Proxy
66 | [Istio Ambient Mesh - Testing out sidecar-less](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/66-Istio%20Ambient%20Mesh%20-%20Testing%20out%20sidecar-less.md) | Tutorial | Sidecar-less operations
67 | [Istio Ambient Mesh - Sidecar and Sidecar-less together](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/67-Istio%20Ambient%20Mesh%20-%20Sidecar%20and%20Sidecar-less%20together.md) | Tutorial | The best of both worlds in Service Mesh
68 | [A Rust-based proxy with Istio Ambient Mesh](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/68-A%20Rust-based%20proxy%20with%20Istio%20Ambient%20Mesh.md) | Informational | The reasoning behind a rust-based proxy.
69 | [Contributing to the Istio Project](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/69-Contributing%20to%20the%20Istio%20Project.md) | Informational | How do we contribute to the Istio project?
70 | [Additional Resources and Playgrounds](https://github.com/distributethe6ix/70DaysOfServiceMesh/blob/main/70DaysExercises/70-Additional%20Resources%20and%20Playgrounds.md) | Informational | MORE INFO =D
---
## 🧰 Contributions
- Contribution is the best way to support and get involved in community !

- Please, consult our [CONTRIBUTING.md](./CONTRIBUTING.md) guide for interacting in our community.
- Please give a ⭐
 



## Thanks to the all Contributors ❤️

<img src="https://contrib.rocks/image?repo=distributethe6ix/70DaysOfServiceMesh" />
