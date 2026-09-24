# Cloud Storage Types Research

## Comparison of Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| **Block Storage** | Data is split into fixed-sized blocks and stored as separate units; each block has its own address. It behaves like a traditional hard drive. | Databases, transactional systems, applications needing low-latency direct disk access | AWS EBS, Azure Disk Storage, GCP Persistent Disk |
| **File Storage** | Data is stored in a hierarchical folder structure with files and directories; multiple users and systems can access it simultaneously. | Shared file storage, home directories, content management systems | AWS EFS, Azure Files, GCP Filestore |
| **Object Storage** | Data is stored as individual objects with unique IDs and rich metadata; organized in buckets instead of folders. Designed for massive scalability. | Images, videos, backups, logs, unstructured data at scale | AWS S3, Azure Blob Storage, GCP Cloud Storage |

## Recommendation for Photo-Sharing Application
Object Storage is the ideal choice for storing millions of user-uploaded photos because it scales infinitely without the performance limits or directory constraints of file-based systems. Each image is stored as a self-contained object with its own unique URL, making it fast to retrieve and simple to distribute worldwide. Unlike block storage, which is tied to a single server, object storage ensures photos remain accessible even if hardware fails — and it costs significantly less at scale.
