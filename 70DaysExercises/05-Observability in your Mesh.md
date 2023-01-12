## 5 - Observability in your Mesh
> **Tutorial**
> *Let's see what's going on in our mesh*

What do you do when an application responds too slowly? Sometimes, there are network conditions well outside of our control, especially in Cloud and Data Center environments where QoS can be challenging to tune. But before we can tune, we need to see what's up.

A Service Mesh provides the right key pieces to capture this data.
The Istio Service Mesh generates a few types of telemetry and metrics to give a sense of what's happening with:
- The control plane
- The data plane
- Services inside of the mesh

Istio provides details around:
- Metrics for latency, errors, traffic and saturation
- Distributed tracing for spans to understand request flows
- Access logs, to determine source/destination metadata of requests.

I have set up specific days to cover deeper observability but, let's get it going and use some tools like:
- Prometheus
- Grafana
- Jaegar
- Kiali 

### Installing the sample observability addons
I'm using the same Civo Kubernetes cluster I've been using since I started this, but I plan to create some automation to turn up and down new clusters.

I'm going to change back to the Istio-1.16.1 directory
```
cd istio-1.16.1
```
And then I'll deploy the sample add-ons provided in the original zip file. 
```
kubectl apply -f samples/addons
```
Give it a couple of minutes and then double check.
```
kubectl get pods -n istio-system
```
```
NAME                                    READY   STATUS    RESTARTS   AGE
istio-egressgateway-7475c75b68-mpxf7    1/1     Running   0          5d15h
istiod-885df7bc9-f9k7c                  1/1     Running   0          5d15h
istio-ingressgateway-6688c7f65d-szxf9   1/1     Running   0          5d15h
jaeger-54b7b57547-vsnhl                 1/1     Running   0          34s
prometheus-7b8b9dd44c-kd77d             2/2     Running   0          32s
grafana-b854c6c8-fhjlh                  1/1     Running   0          35s
kiali-5ff88f8595-fnk8t                  1/1     Running   0          33s
```
Perfect, let's proceed with Prometheus.

### Prometheus 
To get pro
### Grafana

### Jaegar

### Kiali