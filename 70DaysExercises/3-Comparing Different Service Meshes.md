## 3 - Comparing Different Service Meshes
> **Informational**
> *A comparison of Istio, Linkerd, Consul, AWS App Mesh and Cilium*

### Service Mesh Offerings
There are PLENTY of service mesh offerings out there. Some are highly proprietary while others are very open.
Here are offerings you should definitely look into:

Service Mesh | Open Source or Proprietary | Notes |
---|---|---|
Istio | Open Source | Widely adopted and abstracted
Linkerd | Open Source | Built by Buoyant
Consul | Open Source | Owned by Hashcorp, Cloud offering available
Kuma | Open Source | Maintained by Kong
Traefik Mesh | Open Source | Specialized Proxy
Open Service Mesh | Open Source | By Microsoft 
Gloo Mesh | Proprietary | Built by Solo.io ontop of Istio
AWS App Mesh | Proprietary | AWS specific services
OpenShift Service Mesh | Proprietary | Built by Redhad, based on Istio
Tanzu Service Mesh | Proprietary | SaaS based on Istio, built by VMware
Anthos Service Mesh | Proprietary | SaaS based on Istio, built by Google
Bouyant Cloud | Proprietary | SaaS based on Linkerd


I'll quickly recap some of the key options I'll compare. This was taken from Day 1.

#### Istio 
Istio is an open-source service mesh built by Google, IBM, and Lyft, and currently actively developed on and maintained by companies such as Solo.io. It is based on the Envoy proxy which is adopted for the sidecar pattern. Istio offers a high degree of customization and extensibility with advanced traffic routing, observability, and security for microservices. A new mode of operation for sidecar-less service mesh, called Ambient Mesh, was launched in 2022.

#### AppMesh
AppMesh is a service mesh implementation that is proprietary to AWS but primarily focuses in on applications deployed to various AWS services such as ECS, EKS, EC2. Its tight-nit integration into the AWS ecosystem allows for quick onboarding of services into the mesh. 

#### Consul 
Consul is a serivce mesh offering from Hashicorp that also provides traffic routing, observability, and sercurity much like Istio does.

#### Linkerd
Linkerd is an open-source service mesh offering that is lightweight. Similar to Istio, it provides traffic management, observability, and security, using a similar architecture. Linkerd adopts a sidecar-pattern using a Rust-based proxy.

#### Cilium
Cilium is a Container Networking Interface that leverages eBPF to optimize packet processing using the Linux kernel. It offers some Service Mesh capabilities, and doesn't use the sidecar model. It proceeds to deploy a per-node instance of Envoy for any sort of Layer 7 processing of requests. 

Feature | Istio | Linkerd | AppMesh| Consul| Cilium | 
---|---|---|---|---|---|
Current Version | 1.16.1 | 2.12 | N/A (it's AWS :D ) | 1.14.3 | 1.12
Project Creators | Google, Lyft, IBM, Solo | Buoyant | AWS | Hashicorp | Cilium 
Service Proxy | Envoy, Rust-Proxy (experimental) | Linkerd2-proxy | Envoy | Interchangeable, Envoy default | Per-node Envoy
Ingress Capabilities | Yes via the Istio Ingress-Gateway | No; BYO | Yes via AWS | 
Governance and Oversight
Getting Started
Production Ready
Key Features
Pros
Cons
Protocol Support
Sidecar Modes
CNI Redirection
Platform Support
Cloud Support
Multi-workloads
Multi-cluster Mesh
Traffic Management
Monitoring
Resiliency Capabilities
Security Capabilities