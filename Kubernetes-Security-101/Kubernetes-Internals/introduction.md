# Understanding Kubernetes Internals

### Kubernetes Architecture: 
API server ---> etcd ----> scheduler ----> controller manager ----> kubelet ----> kube-proxy.

Pods, services, deployments, namespaces, RBAC, secrets, config maps.

Control plane vs data plane.

# Container Runtime 
Every host OS used for running containers has binaries that establish and maintain the environment for each container, also known as the container runtime. 
Examples: Docker, rkt and OCI  

![Kubernetes Security](image.png)


# External Tools 
kube-bench
AppArmor
seccomp
gVisor
Kata Containers
Trivy
Falco