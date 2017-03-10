# Globally Scalable Microservices with Google Container Engine and Google Load Balancing

## Sidecar container
Container that helps the primary container do it's job.

## Stateful Set
Set of pods that scale horizontally with each pod maintaining a consistent network and disk id.

## Multi-Cluster
* Federation control plane - Servuce that manages global state of federated clusters
* kubefed - CLI tool to administrate federated clusters
* Federated ingress - Native K8S L7 router
* HTTP(S) Load Balancer - Global L7 load balancing

## Sync vs Async
Synchronous is easy to do, k8s makes it even easier. This can be done RESTfully or with RPCs.
