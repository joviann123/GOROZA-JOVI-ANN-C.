# MinIO / S3 Object Storage Deployment Documentation

## 1. Environment & Architecture
Due to environment restrictions in KillerCoda preventing direct Docker image pulls and binary execution, `moto_server` was deployed as a fully S3-compliant Object Storage emulator running directly on the host system.

## 2. Deployment Details
* **Service Executed**: S3 Object Storage Service (`moto_server`)
* **API Endpoint Port**: `9000`
* **Configured Access Key**: `cloudadmin`
* **Configured Secret Key**: `CloudNova2026!`

## 3. Environment Variables & Configuration
* `-p 9000`: Maps and exposes the S3 API endpoint on port 9000.
* `AWS_ACCESS_KEY_ID`: Sets the administrator username/access key (`cloudadmin`).
* `AWS_SECRET_ACCESS_KEY`: Sets the administrator password/secret key (`CloudNova2026!`).
* `AWS_DEFAULT_REGION`: Configured to `us-east-1` for standard S3 API routing.

## 4. Storage & Bucket Management
* **Bucket Created**: `lab-data-bucket`
* **Test File Uploaded**: `test-file.txt`
* **Verification Command**:
  ```bash
  aws --endpoint-url [http://127.0.0.1:9000](http://127.0.0.1:9000) s3 ls s3://lab-data-bucket/
