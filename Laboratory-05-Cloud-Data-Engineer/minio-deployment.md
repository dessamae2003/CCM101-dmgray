# MinIO Deployment Documentation

## Docker Command Used
\`\`\`bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
\`\`\`

## Access Details
- **API Port:** 9000
- **Web Console Port:** 9001
- **Bucket Created:** `client-photos`

## Environment Variables Explanation
The `-e` flags set environment variables inside the container at startup:
- `MINIO_ROOT_USER=cloudadmin` sets the admin username used to log into the MinIO web console.
- `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the admin password for that account.

These credentials secure access to the storage server, ensuring only authorized users can manage buckets and objects.
