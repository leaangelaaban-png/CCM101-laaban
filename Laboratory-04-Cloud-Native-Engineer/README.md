# Laboratory Activity 4 - The Cloud-Native Engineer

## Mission Overview

This laboratory activity focuses on understanding the difference between traditional Virtual Machines and Containers. It also provides hands-on experience in using Docker through the KillerCoda Playground and deploying an Nginx web server inside a container.

## Objectives

- Differentiate Virtual Machines from Containers.
- Access a Docker-enabled environment using KillerCoda.
- Execute basic Docker CLI commands.
- Pull and run an Nginx container.
- Manage the lifecycle of a Docker container.
- Document container operations using Markdown.

## Docker Commands Executed

### Check Docker

`docker --version`

Displays the installed Docker version.

`docker ps`

Displays the currently running containers.

### Deploy Nginx

`docker pull nginx`

Downloads the official Nginx image.

`docker run -d --name nginx-web -p 8080:80 nginx`

Runs the Nginx container in detached mode and maps host port 8080 to container port 80.

`curl http://localhost:8080`

Checks if the Nginx web server is accessible locally.

### Container Lifecycle

`docker ps`

Lists the running containers.

`docker stop nginx-web`

Stops the Nginx container.

`docker ps -a`

Displays all containers, including stopped containers.

`docker rm nginx-web`

Removes the stopped Nginx container.

## Skills Learned

Through this activity, I learned how to use basic Docker commands and manage a container through its lifecycle. I also learned how to pull an image, deploy an Nginx web server, map ports, verify the server, stop a container, and remove it.

## Challenges Encountered

One challenge I encountered was becoming familiar with the Docker commands and understanding what each command does. Following the commands in order helped me understand how a container is deployed and managed.
