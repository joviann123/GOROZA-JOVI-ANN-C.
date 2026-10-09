# Multi-Tier Architecture: Two-Tier Cloud Deployment

## 1. Overview
A multi-tier architecture separates application logic, presentation, and data management into distinct, independent tiers running in isolated environments.

## 2. The Web/Application Tier
* **Role**: Presentation and application processing layer.
* **Responsibilities**: Serves the Nextcloud user interface over HTTP/HTTPS, handles user file uploads, and routes application requests to the backend tier.

## 3. The Database Tier
* **Role**: Persistent data storage layer.
* **Responsibilities**: Manages relational system metadata, user accounts, directory structures, and file indexes inside MariaDB.

## 4. Architectural Separation Rationale
Separating the web application and database into two dedicated containers provides modular scalability, enhanced security, and resource isolation. Isolating them prevents web traffic spikes from exhausting database CPU/RAM resources and restricts database access exclusively to the internal container network.
