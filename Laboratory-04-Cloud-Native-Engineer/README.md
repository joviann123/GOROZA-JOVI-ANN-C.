# Laboratory 04: The Cloud-Native Engineer

## Mission Overview
This activity documents the architectural shift from traditional hardware-level Virtual Machines to lightweight containerization using Docker. As part of CloudNova Technologies, this repository demonstrates container deployment, port mapping, lifecycle management, and hands-on terminal operations on KillerCoda.

---

## Objectives
* Differentiate between traditional Virtual Machines (VMs) and Containers.
* Access a Docker-enabled cloud environment using KillerCoda.
* Execute fundamental Docker CLI commands.
* Pull, run, manage, and terminate a containerized application (Nginx).
* Document container operations using Markdown.

---

## Docker Commands Executed
* `docker --version` & `docker info` - Verified Docker installation and daemon status.
* `docker pull nginx` - Retrieved the official Nginx web server image from Docker Hub.
* `docker run -d -p 8080:80 --name my-nginx nginx` - Deployed Nginx in detached mode mapping host port 8080 to container port 80.
* `curl http://localhost:8080` - Validated web server availability locally via HTTP request.
* `docker ps` - Listed active containers.
* `docker stop my-nginx` - Stopped the running container.
* `docker ps -a` - Verified the container status became exited.
* `docker rm my-nginx` - Removed the container instance completely.

---

## Evidence Screenshots
* **Docker Verification:** `screenshots/docker-version.png`
* **Nginx Deployment:** `screenshots/nginx-running.png`
* **Container Lifecycle:** `screenshots/container-lifecycle.png`

---

## Skills Learned & Challenges Encountered
* **Skills Learned:** Mastered Docker CLI fundamentals, port forwarding, image retrieval, and container lifecycle management.
* **Challenges Encountered:** Understanding host-to-container port binding (`-p 8080:80`) and managing stopped container states before removal.
