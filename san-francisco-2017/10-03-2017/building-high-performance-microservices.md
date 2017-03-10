# Building High Performance Microservices with Go, Kubernetes and gRPC

## Microservice Performance Gotchas
* Slow data serialization
* Network contention
* High per-process overhead

## gRPC
Compact, strongly typed, cross-platform message passing with efficient bi-directional streaming.

## Go
Small footprint runtime, modern and efficient networking.

## Protobufs
Language agnostic, strongly type definition for an API.

Can be automatically translated into client and server libraries for many languages using the `protoc` command.

## Defining a Build Pipeline
Easy way to build pipelines for building images.

Can be invoked from the command line:

```bash
$ gcloud container builds create
```

Or set up a *build trigger* in Google Container Registry to rebuild the image on each commit.

## Where to Next?
* End to end production tracing (Stackdriver Trace)
* Live debugging (Stackdriver Debugger)
* Google Cloud Endpoints (detailed logging, monitoring, centralized access control)
