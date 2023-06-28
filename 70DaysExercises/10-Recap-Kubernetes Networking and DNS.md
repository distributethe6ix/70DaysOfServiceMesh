## 10 - Recap: Kubernetes Networking and DNS
### Tutorial
- Let's dive into Kubernetes Networking and DNS

Kubernetes Networking and DNS are important components of the Kubernetes ecosystem that enable communication and service discovery between containers and services running within a Kubernetes cluster. Let's explore each of these aspects in more detail:

### What is Kubernetes Networking?
In a Kubernetes cluster, containers are deployed across multiple nodes (servers). Kubernetes networking provides a reliable and scalable way for these containers to communicate with each other. It abstracts the underlying network infrastructure and provides a unified network model for containerized applications.

#### Key concepts in Kubernetes networking include:
* Pod: The smallest unit of deployment in Kubernetes, consisting of one or more containers that are co-located and share the same network namespace.
* Service: An abstraction that defines a logical set of pods and provides a stable network endpoint for accessing them. Services enable load balancing and service discovery within the cluster.
* Ingress: A Kubernetes resource that manages external access to services within a cluster. It acts as an entry point and routes incoming traffic to the appropriate services based on defined rules.
