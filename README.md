# Spring Cloud Config Repository

This repository contains configuration files (in YAML format) for use with a **Spring Cloud Config Server**.

Each file defines environment-specific properties for individual microservices in a centralized and version-controlled way.

## Structure

- `application.yaml` – Global configuration for all services.
- `{service-name}.yaml` – Service-specific configuration.
- `{service-name}-{profile}.yaml` – Profile-specific configuration (e.g., `dev`, `prod`).

## Usage

This repo is intended to be used by a Spring Cloud Config Server. Services will fetch their configurations from here at startup.

Example request:
