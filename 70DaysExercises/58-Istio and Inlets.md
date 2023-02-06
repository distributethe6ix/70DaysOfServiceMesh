## 58 - Istio and Inlets
### Tutorial
- Using Inlets for the LoadBalancer Service for Istio Ingress Gateways

I'm currently using Inlets to serve as a way to SSH into Linux node of mine, AND have it act as a Load-balancer for my Istio Ingress Gateway. 

Inlet's an

Install arkade
curl -sLS https://get.arkade.dev | sudo sh
arkade get inletsctl
arkade get inlets-pro


# Obtain a license at https://inlets.dev/pricing
# Store it at $HOME/.inlets/LICENSE or use --help for more options

# Give a single value or comma-separated
export PORTS="8000"

# Where to route traffic from the inlets server
export UPSTREAM="localhost"

inlets-pro tcp client --url "wss://[MY_IP]:8123" \
  --token "[MY_TOKEN]" \
  --upstream $UPSTREAM \
  --ports $PORTS

To delete:
  inletsctl delete --provider digitalocean --id "MY_ID"

SSH
export IP="[MY_IP]"
export TCP_PORTS="2222"
export LICENSE_FILE="$HOME/LICENSE.txt"
export UPSTREAM="localhost"

inlets-pro tcp client --url "wss://$IP:8123/connect" \
  --token "[MY_TOKEN]" \
  --license-file "$LICENSE_FILE" \
  --upstream "$UPSTREAM" \
  --ports $TCP_PORTS


Istio:


arkade install inlets-operator \
 --provider digitalocean \
 --region tor1 \
 --token-file access-token-do-istio \
 --license-file "$HOME/LICENSE.txt”



```
cat kind-config.yaml
```
```
# three node (two workers) cluster config
kind: Cluster
apiVersion: kind.x-k8s.io/v1alpha4
name: edgecompute
nodes:
- role: control-plane
- role: worker
- role: worker
```

cat kind1.yaml 
kind create cluster --config kind-config.yaml 
wget https://storage.googleapis.com/istio-build/dev/0.0.0-ambient.191fe680b52c1754ee72a06b3e0d3f9d116f2e82/istioctl-0.0.0-ambient.191fe680b52c1754ee72a06b3e0d3f9d116f2e82-linux-amd64.tar.gz
tar zxvf istioctl*.tar.gz
./istioctl install -y --set profile=ambient
kubectl get svc -n istio-system
ls
arkade install inlets-operator  --provider digitalocean  --region tor1  --token-file access-token-do-istio  --license-file "$HOME/LICENSE.txt”
arkade install inlets-operator  --provider digitalocean  --region tor1  --token-file access-token-do-istio  --license-file "$HOME/LICENSE.txt"
kubectl get pods
kubectl get svc
kubectl get svc -n istio-system
kubectl get svc -n istio-system -w
kubectl apply -f https://raw.githubusercontent.com/istio/istio/release-1.16/samples/bookinfo/platform/kube/bookinfo.yaml
kubectl apply -f https://raw.githubusercontent.com/linsun/sample-apps/main/sleep/sleep.yaml && kubectl apply -f https://raw.githubusercontent.com/linsun/sample-apps/main/sleep/notsleep.yaml
kubectl apply -f https://raw.githubusercontent.com/istio/istio/release-1.16/samples/bookinfo/networking/bookinfo-gateway.yaml
kubectl get svc -n istio-system -w
kubectl get pods
kubectl get pods -n istio-system
curl ${kubectl get svc istio-ingress-gateway -n istio-system}/productpage
