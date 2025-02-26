# Kata Containers 

Kata containers achieves container isolation by running them in a lightweight virtual machine. 

# gVisor

 gVisor takes a different approach. It effectively implements a Linux kernel that runs on the host system. Therefore, syscalls are not shared anymore across all containers on the host system.