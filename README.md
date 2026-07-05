# E-Commerce Config Repository

This repository contains the centralized configuration files for the E-Commerce Microservices project.

It is used by the Spring Cloud Config Server to provide external configuration for different services such as:

* Product Service
* Inventory Service
* Order Service
* Payment Service
* API Gateway
* Eureka Server

## Purpose

Instead of keeping configuration inside each microservice, this repository acts as a central place for managing service configurations.

The Config Server reads these files from GitHub and provides them to the microservices at runtime.

## Repository Structure

```text
ecommerce-config-repo/
│
├── application.yml
├── product-service.yml
├── inventory-service.yml
├── order-service.yml
└── payment-service.yml
```

## Notes

This repository should not contain real passwords, tokens, private keys, or production secrets.

Sensitive values should be provided using environment variables.
