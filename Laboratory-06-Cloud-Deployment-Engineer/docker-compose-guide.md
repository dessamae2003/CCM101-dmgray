# Docker Compose Technical Guide

## 1. What does the services: block do?
The `services:` block defines the individual containers that will make up your multi-container application stack. Each indented key underneath it (such as `database` and `app`) represents a distinct service container, specifying its container image, environment variables, port mappings, and network relationships.

---

## 2. How did the Nextcloud app container know how to find the database container?
The Nextcloud app container locates the database container using the environment variable `MYSQL_HOST=database`. Docker Compose automatically creates a default user-defined bridge network for the stack, enabling built-in internal DNS resolution where container service names (like `database`) resolve directly to their corresponding internal container IP addresses.

---

## 3. What is the difference between `docker run` and `docker-compose up -d`?
* **`docker run`**: Used to manually launch single standalone containers one by one. It requires typing long, complex command lines specifying individual port mappings, network flags, and environment variables for every single container.
* **`docker-compose up -d`**: Implements Infrastructure as Code (IaC) principles. It reads a declarative YAML configuration file (`docker-compose.yml`) to provision, network, and launch an entire multi-container architecture simultaneously in the background with a single command.
