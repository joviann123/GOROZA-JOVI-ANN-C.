# Laboratory 06: The Cloud Deployment Engineer

## Mission Overview
This mission transitions manual container management to Infrastructure as Code (IaC) principles using Docker Compose. A two-tier private cloud storage solution consisting of Nextcloud (Application Tier) and MariaDB (Database Tier) was declaratively defined and deployed.

## Objectives
* Understand multi-tier web application architecture.
* Construct declarative `docker-compose.yml` Infrastructure as Code files.
* Orchestrate multi-container application stacks via Docker Compose CLI.
* Verify web access routing over exposed container ports.

## Commands Executed
```bash
# Navigate and edit code
mkdir nextcloud-deployment && cd nextcloud-deployment
nano docker-compose.yml

# Deploy stack
docker-compose up -d
docker-compose ps

# Teardown stack
docker-compose down
