# Cloud Storage Types Research

## Storage Comparison Table

| Storage Type | Description (How it stores data) | Primary Use Case (Best used for) | Cloud Provider Example |
| :--- | :--- | :--- | :--- |
| **Block Storage** | Splitting data into fixed-size raw volumes/blocks, each acting as an individual hard drive without metadata. | Operating systems, boot volumes, high-performance transactional databases. | AWS EBS (Elastic Block Store), Azure Managed Disks |
| **File Storage** | Storing data in a hierarchical file system (folders and files) shared over network protocols like NFS/SMB. | Shared network file drives, legacy application migration, content management systems. | AWS EFS (Elastic File System), Azure Files |
| **Object Storage** | Storing data as self-contained units (objects) inside flat address spaces (buckets) with unique IDs and custom metadata. | Unstructured data (images, videos, backups), static website assets, big data analytics. | AWS S3 (Simple Storage Service), MinIO, Azure Blob Storage |

---

## Client Recommendation: Object Storage for User-Uploaded Images

Object Storage is the ideal solution for storing millions of user-uploaded photos because it provides flat, virtually unlimited scalability without the constraints or high cost of expanding fixed block disk volumes. Unlike traditional file systems that struggle with performance degradation under complex folder hierarchies, Object Storage organizes data efficiently with unique identifiers and customizable metadata. Furthermore, separating media storage into an S3-compatible system like MinIO keeps web application containers stateless, lightweight, and capable of scaling independently.
