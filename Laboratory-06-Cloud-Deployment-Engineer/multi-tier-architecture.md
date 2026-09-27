# Multi-Tier Application Architecture

## Web/Application Tier

The Web/Application Tier is the part of the system that users interact with. In this laboratory, Nextcloud provides the application and web interface where users can access the cloud storage system.

## Database Tier

The Database Tier stores the information required by the application. MariaDB is used as the database service for the Nextcloud deployment.

## Why Keep Them Separate?

The application and database are separated into different services so that each component can focus on a specific task. The Nextcloud application can communicate with MariaDB through the Docker network while both services remain independently managed.
