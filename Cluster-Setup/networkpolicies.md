# Network Policies 

1. Kubernetes assigns a unique IP address to every Pod upon creation from the Pod CIDR range of its node. 

2. The IP address is ephemeral and therefore cannot be considered stable over time. 

3. Every restart of a Pod leases a new IP address. 

4. It’s recommended to use Pod-to-Service communication over Pod-to-Pod communication so that you can rely on a consistent network interface.