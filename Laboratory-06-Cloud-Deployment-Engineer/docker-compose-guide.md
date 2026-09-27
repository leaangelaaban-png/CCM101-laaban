# Docker Compose Guide

## The services: Block

The `services:` section contains the different components that Docker Compose will manage. For this deployment, the configuration defines an `app` service for Nextcloud and a `database` service for MariaDB.

## MYSQL_HOST=database

The `MYSQL_HOST=database` variable tells Nextcloud which service provides its database. The word `database` matches the MariaDB service name in the Compose configuration. This allows the application to locate the database through the Docker network.

## docker run vs docker-compose up -d

The `docker run` command can be used when starting and configuring a container individually. The `docker-compose up -d` command is more suitable for this project because the application needs more than one related service. Docker Compose reads the YAML configuration and starts the defined services together in detached mode.
