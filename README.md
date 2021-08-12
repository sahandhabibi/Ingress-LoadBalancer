# Ingress-LoadBalancer
##Ingress Load Balancer via MetalLB

In the first step, install the METALLB service on your Kubernetes cluster. https://metallb.universe.tf
Do the METALLB configuration as follows.

```
metallb_enabled: true
metallb_ip_range:
  - "10.0.70.100-10.0.70.132" # Choose IP range MetalLB can give out on the L2 network segment
metallb_protocol: "layer2"

```


refrence: https://imranh.co.uk/2020/05/21/kubespray-ingress-loadbalancer.html 
