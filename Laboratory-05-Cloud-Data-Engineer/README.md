# Laboratory 05: The Cloud Data Engineer

## Mission Overview
This laboratory activity focuses on deploying, configuring, and verifying a cloud-native S3-compatible Object Storage service. The objective is to simulate a cloud data engineering workspace by managing storage buckets, setting access credentials, and performing programmatic object storage verification.

## Objectives
* Deploy an S3-compliant Object Storage server (`moto_server`/MinIO API) on port 9000.
* Configure administrative access credentials (`cloudadmin` / `CloudNova2026!`).
* Create a persistent storage bucket (`lab-data-bucket`).
* Perform object ingestion and read verification using the AWS CLI tool.
* Capture and archive terminal artifacts in the repository.

## Tools Used
* **Ubuntu 24.04 LTS (KillerCoda Environment)**
* **Python / Moto Server (S3 API Emulator)**
* **AWS CLI (S3 Client Integration)**
* **Bash Shell & Network Diagnostic Utilities (`netstat`, `ps`)**

## Skills Learned
* Deploying and managing S3-compatible Object Storage services.
* Network port binding and process verification in Linux environments.
* Programmatic interaction with Object Storage using AWS CLI endpoints.
* Managing cloud credentials and environment variables securely.

## Visual Verification
* **Deployed Object Storage Status**: `screenshots/minio-deployed.png`
* **Bucket Creation & File Upload**: `screenshots/minio-bucket-upload.png`
