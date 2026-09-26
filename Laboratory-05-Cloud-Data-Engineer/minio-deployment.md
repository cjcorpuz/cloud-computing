# MinIO Deployment

## Docker Deployment

MinIO was deployed using Docker in the KillerCoda Ubuntu Playground. The following command was used:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
elestio/minio:latest server /data --console-address ":9001"
```

## Web Console Port

The MinIO web console was accessed through port **9001** using the KillerCoda port access feature.

## Bucket Created

A bucket named **client-photos** was created in the MinIO Object Browser. A sample image was uploaded successfully to the bucket.

## Environment Variables

The `-e` option is used to set environment variables for the MinIO container.

* `MINIO_ROOT_USER=cloudadmin` sets the administrator username.
* `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the administrator password.

These variables provide the login credentials needed to access the MinIO web console.
