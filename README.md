# Deployment pipeline for a microservice-based e-shop application

## Application

Here we use an e-shop application that contains several micro-services as an example. Each service exposes a set of APIs, some of which are public while the others are for internal use only. The application uses a database for data storage.

### Service list:

- user-service
  - POST /api/v1/login (public)
  - POST /api/v1/logout (public)
  - POST /api/v1/signup (public)
- product-service
  - GET /api/v1/products (public)
- payment-service
  - POST /api/v1/pay (public)
  - POST /api/v1/cancel (internal)
- db-service
  - GET, POST, DELETE /api/v1/user (internal)
  - GET, POST, DELETE /api/v1/creditcard (internal)
  - GET, POST, DELETE /api/v1/product (internal)

### Production environment requirements

- People can access this application via a domain name such as www.happyshopping.com
- The payment service needs to support different vendors like Visa, Mastercard, AMEX, etc
- It should be fast
- It should be secure
- It should have high availability
- It should be able to scale based on workloads
- It must run within Kubernetes cluster

## Dependencies of the micro-services

## Thoughts of the production environment requirements

## Proposed deployment architecture

## TODO
- [ ] architecture with diagrams and explanations
- [ ] K8s manifest files
