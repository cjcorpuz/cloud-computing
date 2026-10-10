# Docker Compose Guide

## 1. What Does the `services:` Block Do?

The `services:` block defines the containers or services that Docker Compose will manage. In our project, there are two services: `database` and `app`.

- **Database Service:** Uses the `mariadb:10.6` image to store Nextcloud data.
- **App Service:** Uses the `nextcloud` image to run the Nextcloud web application and exposes port `8080` on the host to port `80` inside the container.

Using the `services:` block allows both containers to be configured and managed through a single YAML file.

## 2. How Does Nextcloud Find the Database Container?

The Nextcloud application finds the database through the `MYSQL_HOST` environment variable.

```yaml
MYSQL_HOST=database
```

The value `database` matches the name of the database service in the Docker Compose file. Docker Compose creates a shared network for the services, allowing the Nextcloud container to locate the MariaDB container using its service name.

This makes communication between the application and database easier without manually entering the database container's IP address.

## 3. Difference Between `docker run` and `docker-compose up -d`

### Docker Run

The `docker run` command starts an individual container. Its configuration, such as the image, ports, and environment variables, is usually specified through command-line options.

Example:

```bash
docker run -d -p 8080:80 nextcloud
```

### Docker Compose

The `docker-compose up -d` command starts the services defined in the `docker-compose.yml` file. It can create and run multiple connected containers, such as Nextcloud and MariaDB, using one command.

The `-d` option runs the containers in the background.

Example:

```bash
docker-compose up -d
```

### Summary

Docker Run is useful for starting individual containers, while Docker Compose is more convenient for deploying applications that require multiple connected services. In this mission, Docker Compose was used to manage Nextcloud and MariaDB together.
