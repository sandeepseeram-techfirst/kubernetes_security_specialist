# Kube-bench

Kube-bench is a tool to check Kubernetes cluster components against the CIS Benchmark best practices in an automated fashion. 


kubectl apply -f https://raw.githubusercontent.com/aquasecurity/kube-bench/\
main/job-master.yaml

job.batch/kube-bench-master created


$ kubectl get pods
NAME                      READY   STATUS      RESTARTS   AGE
kube-bench-master-8f6qh   0/1     Completed   0          45s