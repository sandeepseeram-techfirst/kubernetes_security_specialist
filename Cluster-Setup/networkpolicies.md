# Network Policies 

1. Kubernetes assigns a unique IP address to every Pod upon creation from the Pod CIDR range of its node. 

2. The IP address is ephemeral and therefore cannot be considered stable over time. 

3. Every restart of a Pod leases a new IP address. 

4. It’s recommended to use Pod-to-Service communication over Pod-to-Pod communication so that you can rely on a consistent network interface.


##### Network policies act similarly to firewall rules, but for Pod-to-Pod communication. Rules can include the direction of network traffic (ingress and/or egress) for one or many Pods within a namespace or across different namespaces, as well as their targeted ports.

Network policies heavily work with label selection to define rules.

$ kubectl get ns g04 --show-labels
NAME   STATUS   AGE   LABELS
g04    Active   12m   app=orion,kubernetes.io/metadata.name=g04

$ kubectl get pods -n g04 --show-labels
NAME       READY   STATUS    RESTARTS   AGE     LABELS
backend    1/1     Running   0          9m46s   tier=backend
frontend   1/1     Running   0          9m46s   tier=frontend