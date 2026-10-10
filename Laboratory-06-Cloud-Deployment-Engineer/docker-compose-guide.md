# Docker Compose Guide

## Introduction
Docker Compose is a tool used to define and manage multi-container Docker applications through a YAML configuration file.

## Purpose of docker-compose.yml
The `docker-compose.yml` file defines the services, images, environment variables, ports, networks, and volumes needed by an application.

## Services Used

### 1. MariaDB
MariaDB serves as the database service for Nextcloud. It stores application data such as user information and file metadata.

### 2. Nextcloud
Nextcloud provides the web interface for the private cloud storage application. It connects to MariaDB to access database information.

## Important Docker Compose Commands

```bash
docker compose up -d
```
Creates and starts the services in the background.

```bash
docker compose ps
```
Displays the status of the services.

```bash
docker compose logs
```
Displays service logs for troubleshooting.

```bash
docker compose down
```
Stops and removes the containers and network created by Compose. Named volumes are retained unless explicitly removed.

## Benefits of Docker Compose
- Deploys multiple services using one configuration file.
- Simplifies application management.
- Makes deployment more repeatable.
- Supports Infrastructure as Code principles.

## Conclusion
Docker Compose simplifies the deployment and management of multi-container applications such as Nextcloud and MariaDB.
