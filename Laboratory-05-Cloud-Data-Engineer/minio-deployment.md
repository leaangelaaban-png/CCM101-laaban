# My MinIO Cloud Storage Setup

## Deployment

For this activity, I deployed MinIO using Docker to create an S3-compatible object storage environment. The MinIO image stated in the activity could not be pulled in the current KillerCoda environment, so I used the available image from `quay.io` while keeping the required ports, credentials, and server settings.

## Docker Command Used

`docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"`

The command started a container named `minio-server`. Port `9000` was used for the MinIO API, while port `9001` was used for the web console.

## Accessing the Console

I opened the MinIO web console through port `9001`. This allowed me to manage the storage server through a browser after starting it from the command line.

## Bucket and Upload

I created a bucket named `client-photos`. After creating the bucket, I uploaded a sample file to confirm that objects could be stored successfully.

## Environment Variables

The `-e` options were used to provide environment variables when the container started. `MINIO_ROOT_USER` set the root username, while `MINIO_ROOT_PASSWORD` set the password used to access the MinIO console.
