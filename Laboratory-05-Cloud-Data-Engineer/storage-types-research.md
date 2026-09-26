# Cloud Storage Types Research

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-size blocks that can be accessed individually. | Best used for virtual machines, databases, and applications that need fast and consistent storage. | AWS EBS |
| File Storage | Stores data as files in a hierarchical folder structure and allows multiple users or systems to access shared files. | Best used for shared files, documents, and applications that require a common file system. | AWS EFS |
| Object Storage | Stores data as objects together with metadata and a unique identifier. | Best used for large amounts of unstructured data such as images, videos, and backups. | AWS S3 |

## Why Object Storage?

Object Storage is the best choice for the client's photo-sharing application because it is designed to store massive amounts of unstructured data such as images. It can provide scalable and accessible storage for the millions of photos uploaded by users.
