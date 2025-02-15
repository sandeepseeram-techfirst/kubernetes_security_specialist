# Kubernetes Security Contexts 

Both core Kubernetes and the Kubernetes ecosystem offer solutions for defining, enforcing, and governing security settings on the Pod and container level. 

1. Pod Security Admission
2. Open Policy Agent Gatekeeper.


Kubernetes, as the container orchestration engine, can apply additional configuration to increase container security. You do so by defining a security context. 

A security context defines privilege and access control settings for a Pod or a container. 


Kubernetes establishes a clear separation between the container namespace and the host namespace for processes, network, mounts, user ID, and more.