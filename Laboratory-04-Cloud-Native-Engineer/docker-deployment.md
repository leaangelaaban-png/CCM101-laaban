# Docker Deployment and Container Lifecycle

## Nginx Deployment

### Pull the Nginx Image

`docker pull nginx`

This command downloaded the official Nginx image that was used to create the web server container.

### Run the Nginx Container

`docker run -d --name nginx-web -p 8080:80 nginx`

This command started the Nginx container in detached mode and mapped port 8080 of the host to port 80 of the container.

### Test the Web Server

`curl http://localhost:8080`

This command sent a local HTTP request to verify that the Nginx web server was running successfully.

## Container Lifecycle

### List Running Containers

`docker ps`

This command displayed the containers that were currently running.

### Stop the Container

`docker stop nginx-web`

This command stopped the running Nginx container.

### Verify the Container is Stopped

`docker ps -a`

This command displayed all containers and confirmed that the Nginx container had stopped.

### Remove the Container

`docker rm nginx-web`

This command completely removed the stopped Nginx container.
