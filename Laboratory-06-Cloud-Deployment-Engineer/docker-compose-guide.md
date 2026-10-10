# Docker Compose Guide

## 1. What Does the `services:` Block Do?

The `services:` block defines the containers that Docker Compose will create and manage. In our project, there are two services: `database` and `app`.

- **Database Service:** Uses the `mariadb:10.6` image to store Nextcloud data.
- **App Service:** Uses the `nextcloud` image to provide the Nextcloud web application and makes it accessible through port `8080`.

Docker Compose manages both services using one YAML configuration file.

## 2. How Does Nextcloud Find the Database?

The Nextcloud application uses the `MYSQL_HOST` environment variable to identify the database server.

In our YAML file, we configured:

```yaml
MYSQL_HOST=database
```

The value `database` matches the name of the database service in the `services:` block. Docker Compose provides network-based service discovery, allowing the Nextcloud container to communicate with the MariaDB container using that service name.

The database credentials, database name, and username must also match between the two services so Nextcloud can connect successfully.

## 3. Difference Between `docker run` and `docker-compose up -d`

### Docker Run

The `docker run` command starts an individual container using options supplied in the command. Each container's configuration is commonly specified separately.

### Docker Compose

The `docker-compose up -d` command creates and starts the services defined in the `docker-compose.yml` file. It can manage multiple connected containers, their environment variables, port mappings, and network configuration together.

The `-d` option runs the containers in detached mode, allowing them to continue running in the background.

### Conclusion

Docker Compose is useful for multi-container applications such as Nextcloud and MariaDB because it keeps the configuration in one file and simplifies deployment and management.

## 4. Commands Used

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose config
docker-compose up -d
docker-compose ps
docker-compose down
```

These commands were used to create the project directory, configure and validate the YAML file, deploy the containers, check their status, and shut down the infrastructure.
