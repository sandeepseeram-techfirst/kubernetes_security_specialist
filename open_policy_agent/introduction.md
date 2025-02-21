# Open Policy Agent (OPA) and Gatekeeper

Open Policy Agent (OPA) is an open source, general-purpose policy engine for enforcing rules. OPA is not specific to Kubernetes and can be used across other technology stacks.

You can write your own rules with the help of the query language named Rego. The validation logic written in Rego determines if the object is accepted or denied.

Gatekeeper is an extension to Kubernetes that uses OPA. Gatekeeper allows for defining and enforcing custom policies for any kind of Kubernetes API primitive.