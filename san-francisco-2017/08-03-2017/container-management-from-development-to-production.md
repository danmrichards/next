# Container Management and Deployment - From Development to Production

## Cloud Native Applications
* 12 Factor
* Scale horizontally
* Built in monitoring and metrics
* Operability

Microservices not required; monoliths welcome!

## Trace
Tool in GCP to trace application usage and requests

## Google Cloud Container Builder
Build container images from source code

* REST API
* Fully managed service
* Build triggers
* Custom builds (support for custom scripts and container images)
* Google Container Registry integration

`gcloud container builds submit --config=path/to/config.yaml`

## Google Container Registry
Private registry for container images

* Private by default
* IAM integration
* Built on Google Cloud Storage
* Automatic image vulnerability scanning
* List image tags and names
* Docker v2 image format (support for OCI image format on the roadmap)

`gcloud beta container images list-tags path/to/image`

## Google Container Engine
### Managing Development Environments
* Uses shared clusters
* Use namespaces for Environments
* Use resource quotas
    * Define via yaml manifest. Apply to a cluster via `kubectl`
* Allow direct access and self service

### Managing Production Environments
* Use dedicated clusters
* Use resource requests and limits
* Use namespaces for API isolation
* Use health and readiness checks
* Disable direct access (limit access and use a CI system to push changes)

## Misc
Quick way to connect to pod if service is not up yet:

`kubectl port-forward POD_NAME LOCAL_PORT:REMOTE_PORT`
