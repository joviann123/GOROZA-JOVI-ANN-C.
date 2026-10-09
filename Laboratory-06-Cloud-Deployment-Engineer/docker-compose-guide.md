# Docker Compose Technical Guide

## 1. The `services:` Block
The `services:` block defines the distinct containerized components that constitute the multi-tier application architecture. In our configuration, it specifies two isolated microservices: `database` (MariaDB) and `app` (Nextcloud).

## 2. Container Service Discovery (`MYSQL_HOST`)
The Nextcloud container locates the MariaDB container via Docker's internal DNS routing. By setting `MYSQL_HOST=database`, Docker Compose automatically routes network traffic from the web container to the IP address assigned to the service named `database` within the shared default network bridge.

## 3. Difference: `docker run` vs `docker-compose up -d`
* **`docker run`**: Executes and manages individual containers manually one command at a time. It requires manually configuring network bridges, environment variables, and storage volume bindings for each container.
* **`docker-compose up -d`**: Reads a declarative Infrastructure as Code (IaC) YAML specification to build, configure, link, and deploy an entire multi-container stack in the background using a single command.
