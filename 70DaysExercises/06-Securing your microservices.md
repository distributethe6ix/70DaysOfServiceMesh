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
One of the key aspects of the Istio service mesh is its ability to issue and manage identity for workloads that are deployed into the mesh. To put it into perspective, if all services have a sidecar, and are issued an identity (it's own identity) from the Istiod control plane, a new ability to trust and verify services now exists. This is how Peer Authentication is achieved using mTLS. I plan to go into lots more details in future modules.

In Istio, Peer Authentication must be configured for services and can be scoped to workloads, namespaces, or the entire mesh.

There are three modes, I'll explain them briefly and we'll get to configuring!
* PERMISSIVE: for when you have plaintext AND encrypted traffic. Migration-oriented
* STRICT: Only mTLS enabled workloads
* DISABLE: No mTLS at all.

We can also take care of End-user Auth using JWT (JSON Web Tokens) but I'll explore this later.

### Configuring Istio Peer AuthN and Strict mTLS
Let's get to configuring our environment with Peer Authentication and verify.

We already have our environment ready to go so we just need to deploy another sample app that won't have the sidecar, and we also need to turn up an Authentication policy.

Let's deploy a new namespace called sleep and deploy a sleeper pod to it.
```
kubectl create ns sleep
```
```
kubectl get ns
```
```
cd istio-1.16.1
kubectl apply -f samples/sleep/sleep.yaml -n sleep
```

Let's test to make sure the sleeper pod can communicate with the bookinfo app!
This command simply execs into the name of the sleep pod with the "app=sleep" label in the sleep namespace and proceeds to curl productpage in the default namespace. 
The status code should be 200!
```
kubectl exec "$(kubectl get pod -l app=sleep -n sleep -o jsonpath={.items..metadata.name})" -c sleep -n sleep -- curl productpage.default.svc.cluster.local:9080 -s -o /dev/null -w "%{http_code}\n"
```
```
200
```

Let's apply our PeerAuthentication
```
kubectl apply -f - <<EOF
apiVersion: security.istio.io/v1beta1
kind: PeerAuthentication
metadata:
  name: "default"
  namespace: "istio-system"
spec:
  mtls:
    mode: STRICT
EOF
```

Now, if we re-run the curl command as I did previously (I just up-arrowed but you can copy and paste from above), it will fail with exit code 56. This strongly implies that peer-authentication in STRICT mode disallows non-mTLS workloads from communicating with mTLS workloads.

As I mentioned previously, I'll expand further in future days.

### Istio Layer 7 Authorization 

### Configuring L7 Authorization Policies


