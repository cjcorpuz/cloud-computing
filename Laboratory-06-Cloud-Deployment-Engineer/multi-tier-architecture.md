# Multi-Tier Application Architecture

## What is a Two-Tier Architecture?

A Two-Tier Architecture is an application design that separates an application into two main parts: the Web/Application Tier and the Database Tier. In this mission, Nextcloud serves as the web application, while MariaDB manages the database.

## 1. The Web/Application Tier

The Web/Application Tier is responsible for displaying the user interface and handling HTTP requests from users through a web browser. In this project, Nextcloud runs inside a Docker container and allows users to upload, download, organize, and manage their files.

## 2. The Database Tier

The Database Tier is responsible for storing and managing persistent data, such as user account information and file metadata. In this project, MariaDB runs in a separate Docker container and provides the database services required by Nextcloud.

## 3. Why Separate Them?

Separating the web application and database into two containers makes the system easier to manage, maintain, and troubleshoot because each service has its own responsibility. It also allows the services to be updated or scaled independently and helps isolate the database from direct public access. This separation improves organization and security when combined with proper network configuration and access controls.
