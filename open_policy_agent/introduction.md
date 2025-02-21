# Open Policy Agent (OPA) and Gatekeeper

Open Policy Agent (OPA) is an open source, general-purpose policy engine for enforcing rules. OPA is not specific to Kubernetes and can be used across other technology stacks.

You can write your own rules with the help of the query language named Rego. The validation logic written in Rego determines if the object is accepted or denied.

Gatekeeper is an extension to Kubernetes that uses OPA. Gatekeeper allows for defining and enforcing custom policies for any kind of Kubernetes API primitive.

### Installing Gatekeeper

Installing Gatekeeper is relatively easy. All you need to do is to create a bunch of Kubernetes objects from a YAML manifest provided by the Gatekeeper project.

$ kubectl apply -f https://raw.githubusercontent.com/open-policy-agent/\
gatekeeper/master/deploy/gatekeeper.yaml

Gatekeeper objects have been installed in the namespace gatekeeper-system. Make sure that all Pods in the namespace transition into the “Running” status before trying to use Gatekeeper:

$ kubectl get namespaces
NAME                STATUS   AGE
default             Active   29h
gatekeeper-system   Active   4s
...


