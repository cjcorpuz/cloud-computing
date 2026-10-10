# Mission 6: The Cloud Deployment Engineer

## Mission Overview

This mission focuses on deploying a private cloud application using Docker Compose. I deployed Nextcloud as the application service and MariaDB as the database service. I also verified the running containers, accessed the Nextcloud installation page, and shut down the infrastructure after testing.

## Objectives

- Understand the concept of a two-tier architecture.
- Create and validate a `docker-compose.yml` file.
- Deploy Nextcloud and MariaDB using Docker Compose.
- Verify the status of the containers.
- Access the Nextcloud web installation page.
- Safely stop and remove the containers.
- Document the deployment process and commands used.

## Commands Executed

### 1. Create and Access the Project Directory

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
pwd
```

### 2. Validate the Docker Compose Configuration

```bash
docker-compose config
```

### 3. Deploy the Services

```bash
docker-compose up -d
```

### 4. Check the Container Status

```bash
docker-compose ps
```

### 5. Shut Down the Infrastructure

```bash
docker-compose down
```

## Skills Learned

- Creating and managing Docker Compose configuration files.
- Deploying multiple connected containers.
- Understanding application and database services in a two-tier architecture.
- Using environment variables to configure application connections.
- Verifying container status and troubleshooting basic errors.
- Accessing a web application through an exposed port.
- Shutting down containers and documenting deployment results.
