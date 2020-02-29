# Accounting Service
## Table of Contents

- [Description](#description)
- [Documentation](#documentation)
- [Features](#features)
- [Requirements](#requirements)
- [Quick Start / Setup](#quick-start--setup)
- [Configuration](#configuration)

## Description
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/asys1920/accountingservice)](https://github.com/asys1920/accountingservice/releases/tag/v1.0.0)

This microservice is part of the car-rental project which was built
by the Asys course 19/20 at the TH Bingen.

It acts as an API gateway and routes requests to the correct microservices.

The Microservice can be monitored by Prometheus.

Logs can be sent to Elasticsearch/Logstash using Filebeat.

## Documentation
See [Management project](https://github.com/asys1920/management) for a documentation of the whole Car-Rental project.
## Features
This microservice acts as an API gateway and routes requests to the correct microservices.
## Requirements
A JDK with at least Java Version 11.

### Local
### Docker
## Quick Start / Setup
### Run Local
### Run Docker

## Configuration
You can set the Port of the API gateway using the `GATEWAY_PORT` environment variable.
The default Port used by the application is `8080`. To set the address the API gateway
listens on you can use the `GATEWAY_ADDRESS` environment variable, its default value is
`localhost`.

Furthermore, you can set the Addresses of the microservices the gateway routes to using the environment
variables listed below:

Environment Variable | Default Value
--- | --- 
ORDER_ADDRESS | 127.0.0.1
ORDER_PORT | 8081
PAYMENT_ADDRESS | 127.0.0.1
PAYMENT_PORT | 8082
CAR_ADDRESS | 127.0.0.1
CAR_PORT | 8083
USER_ADDRESS | 127.0.0.1
USER_PORT | 8084
ACCOUNTING_ADDRESS | 127.0.0.1
ACCOUNTING_PORT | 8085