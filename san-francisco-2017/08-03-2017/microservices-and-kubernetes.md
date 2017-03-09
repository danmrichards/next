# Microservices and Kubernetes - New functionality to assemble and operate applications at a higher level

## Principles
* Services, not infrastructure
* Interoperability
* Automate everything

## The Service Abstraction

Service Broker --> Service Class --> Service Instance --> Binding

### Service Broker
A clean abstraction that allows services to expose a catalog of capabilities as well as the ability to create, use and delete those services. See "Open Service Broker API".

### Service Class
Factories for provisioning a service instance for consumption.

### Binding
How you connect to and use a service instance

## Service Mesh
Networking for services, not bytes.

* Reliability
* Performance
* Visibility
* Control
