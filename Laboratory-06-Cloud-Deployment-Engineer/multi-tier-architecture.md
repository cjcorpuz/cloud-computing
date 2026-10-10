# Multi-Tier Application Architecture

## Introduction
A multi-tier application architecture divides an application into separate layers. Each layer has a specific responsibility and communicates with the other layers.

## Architecture Components

### 1. Frontend – Nextcloud
Nextcloud provides the web interface that allows users to access and manage their files through a browser.

### 2. Backend – MariaDB
MariaDB stores the database information used by Nextcloud, including user information and file metadata.

### 3. Docker Compose
Docker Compose defines and manages the Nextcloud and MariaDB services using a YAML configuration file.

## How the Components Work Together
1. The user accesses Nextcloud through a web browser.
2. The Nextcloud container processes the user's request.
3. Nextcloud communicates with MariaDB through a private Docker network.
4. MariaDB returns the requested database information to Nextcloud.

## Benefits
- Organized application components.
- Easier deployment and management.
- Better separation of responsibilities.
- Persistent data through Docker volumes.

## Conclusion
The Nextcloud and MariaDB deployment demonstrates how multiple containers work together to provide a private cloud storage application.
