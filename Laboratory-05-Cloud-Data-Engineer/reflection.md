## Mission 5 Reflection
This lab shifted my focus from deploying applications to deploying the storage layer behind them, and it gave me a much better understanding of why object storage has become the standard for cloud-native applications.

# 1. Why is object storage better suited for storing millions of photos compared to a traditional block storage hard drive?
Object storage is far better suited for storing millions of photos than a traditional block storage hard drive because it doesn't rely on a fixed file system hierarchy or a single attached disk. Block storage is designed for structured, high-performance access from one server at a time, which becomes a bottleneck when you need to store and retrieve massive, ever-growing amounts of unstructured data like images. Object storage instead treats each file as an independent object with its own metadata and unique identifier, stored in a flat address space that can scale horizontally across many servers. This means the storage capacity isn't tied to a single disk's limits, and objects can be retrieved directly over HTTP from anywhere, which is exactly what a photo-sharing application needs.

# 2. How did using Docker make it easier to deploy the MinIO storage server?
Docker made deploying MinIO significantly easier than a manual installation would have been. Instead of downloading binaries, configuring storage paths, and setting up networking by hand, a single `docker run` command pulled the entire MinIO server, mapped both the API port and the web console port, and set the login credentials through environment variables. This was also where I ran into a real-world issue: the original `minio/minio` image had been removed from Docker Hub, so I had to research the error, find that MinIO had moved distribution to quay.io, and adjust the image reference accordingly. That troubleshooting reinforced how much containerized deployments still depend on understanding what's actually happening under the hood, not just copying commands.

# 3. What is a "bucket" in the context of cloud storage?
A "bucket" in cloud storage is the top-level container that holds objects, similar to a root folder, but without the nested folder structure of traditional file systems. Every object uploaded to MinIO or S3 must belong to a bucket, and buckets are also where access policies and permissions are typically configured.

# 4. How do you think large enterprise companies ensure their object storage data is not lost if the physical server crashes?
For large enterprises, protecting against data loss usually means replicating data across multiple physical disks, servers, and often entirely separate data centers or geographic regions, so that a single hardware failure never results in permanent loss. Techniques like erasure coding, versioning, and automated backups are commonly layered on top of this replication.

# 5. How is your confidence in navigating the Linux command line growing? 
My confidence in the Linux command line keeps growing with each lab. Between managing Docker containers in Lab 4 and troubleshooting a failed image pull in this lab, I'm getting more comfortable reading error messages, understanding what they actually mean, and adjusting my approach instead of getting stuck.
