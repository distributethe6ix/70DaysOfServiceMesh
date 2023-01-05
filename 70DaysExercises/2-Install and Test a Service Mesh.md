## 2 - Install and Test a Service Mesh
> **Tutorial**
> *Let's install our first service mesh.*

### Installation Prequisites
- A Kubernetes cluster running 1.22, 1.23, 1.24, 1.25
    - KinD
    - Minikube
    - Civo K8s
    - EKS
- Access to a Loadbalancer service
    - Metallb
    - port-forwarding (not preferred)
    - Cloud Load-balancer
    - Inlets
- Linux or macOS to run istoctl

1. Verify your cluster is up and operational
    ```
    kubectl get nodes -o wide
    kubectl get pods -A
    ```
2. Download Istio
    ```
    curl -L https://istio.io/downloadIstio | sh -
    ```
3. Change to the Istio directory
    ```
    cd istio-1.16.1
    ```
4. Add the istioctl binary to your path
    ```
    export PATH=$PWD/bin:$PATH
    ```
5. Check to verify that your environment is ready to go:
    ```
    istioctl x precheck
    ```
    And the output
    ```
    ✔ No issues found when checking the cluster. Istio is safe to install or upgrade!
    To get started, check out https://istio.io/latest/docs/setup/getting-started/    
    ```
6. Let's proceed to install Istio
    ```
    istioctl install --set profile=demo -y
    ```
    You will see the following output:
    ```
    ✔ Istio core installed                                                                                                                                                          
    ✔ Istiod installed                                                                                                                                                              
    ✔ Egress gateways installed                                                                                                                                                     
    ✔ Ingress gateways installed                                                                                                                                                    
    ✔ Installation complete 
    ```

