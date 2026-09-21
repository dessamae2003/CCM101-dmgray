# Types of Cloud Storage

## Comparison Table

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Splits data into fixed-size blocks and stores them on a raw disk volume, similar to a traditional hard drive. The OS manages the file system on top. | High-performance workloads needing low latency, like databases and boot volumes | AWS EBS |
| File Storage | Organizes data in a hierarchical folder/file structure and is accessed over a shared network protocol (e.g., NFS, SMB) | Shared file access across multiple servers or users, such as content management systems | AWS EFS |
| Object Storage | Stores data as discrete objects (data + metadata + unique ID) in a flat address space, accessed via HTTP/API rather than a file path | Massive amounts of unstructured data — images, videos, backups, static website assets | AWS S3 |

## Why Object Storage for This Client

Object storage is the best fit for the client's user-uploaded images because it scales virtually infinitely without the need to manage complex file hierarchies or provision fixed disk sizes in advance. Each image is stored as an independent object accessible via a simple URL/API call, which makes it easy to serve directly to end users at scale. Unlike block storage, which is tied to a single server and limited by its provisioned capacity, object storage separates storage from compute, so the photo-sharing app can grow to millions of images without re-architecting the storage layer.
