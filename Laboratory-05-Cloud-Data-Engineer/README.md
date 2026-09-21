# Laboratory 05: Cloud Data Engineer

## Mission Overview
This lab covers deploying an S3-compatible object storage server (MinIO) using Docker, and using it to create a storage bucket and upload a file simulating a real-world photo-sharing app backend.

## Objectives
- Differentiate between Block, File, and Object Storage
- Deploy an S3-compatible Object Storage server (MinIO) using Docker
- Access a cloud service via a web interface using port forwarding
- Create a storage bucket and upload objects to the cloud
- Document cloud storage operations using Markdown

## Tools Used
- Docker
- MinIO (S3-compatible object storage)
- KillerCoda Playground

## Skills Learned
- How to differentiate between Block, File, and Object Storage and identify which use cases each is best suited for.
- How to deploy a multi-container service using Docker with multiple exposed ports (API port 9000 and Web Console port 9001) in a single `docker run` command.
- How to use environment variables (`-e` flags) in Docker to securely set login credentials at container startup.
- How to troubleshoot a failed image pull, including diagnosing a "pull access denied" error and finding an alternative registry (quay.io) when an image was removed from Docker Hub.
- How to access a containerized web service running inside a remote cloud environment using port forwarding through KillerCoda's Traffic/Ports feature.
- How to navigate an S3-compatible object storage web console, including creating a storage bucket and uploading files to it.
- A clearer understanding of how object storage systems like MinIO and Amazon S3 organize data using buckets rather than traditional folder hierarchies.
