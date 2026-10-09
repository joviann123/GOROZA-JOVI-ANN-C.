# Laboratory 06: The Cloud Deployment Engineer

## Mission Overview
This mission transitions manual container management to Infrastructure as Code (IaC) principles using Docker Compose. A two-tier private cloud storage solution consisting of Nextcloud (Application Tier) and MariaDB (Database Tier) was declaratively defined and deployed.

## Objectives
* Understand multi-tier web application architecture.
* Construct declarative `docker-compose.yml` Infrastructure as Code files.
* Orchestrate multi-container application stacks via Docker Compose CLI.
* Verify web access routing over exposed container ports.

## Commands Executed
- Navigate and create folder: `mkdir nextcloud-deployment && cd nextcloud-deployment`
- Create compose file: `nano docker-compose.yml`
- Deploy stack: `docker-compose up -d`
- Check running containers: `docker-compose ps`
- Teardown stack: `docker-compose down`

## Skills Learned
* Multi-tier infrastructure architecture modeling.
* Infrastructure as Code (IaC) authoring in YAML format.
* Docker internal DNS service discovery and container linking.
* Automated application stack deployment and lifecycle management.

## Visual Evidence
* **Deployment Verification**: `screenshots/compose-deployment.png`
* **Nextcloud Web Interface**: `screenshots/nextcloud-web.png`
* **Stack Teardown**: `screenshots/compose-teardown.png`
