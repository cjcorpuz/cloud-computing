# Mission 4: The Cloud-Native Engineer

## Mission Overview

This laboratory activity focused on understanding cloud-native technologies, particularly Docker containers. The activity included comparing virtual machines and containers, deploying an Nginx web server using Docker, and managing the container lifecycle.

## Objectives

- Differentiate virtual machines from containers.
- Use Docker commands to pull and run containers.
- Deploy an Nginx web server using Docker.
- Manage the lifecycle of a Docker container.
- Document Docker commands and their results.

## Docker Commands Executed

### Checkpoint 3 - Verify Docker

```bash
docker --version
docker info
```

### Checkpoint 4 - Deploy Nginx

```bash
docker pull nginx
docker run -d -p 8080:80 --name my-nginx nginx
docker ps
curl http://localhost:8080
```

### Checkpoint 5 - Container Lifecycle

```bash
docker ps
docker stop my-nginx
docker ps
docker rm my-nginx
```

## Skills Learned

Through this activity, I learned how to use Docker CLI commands, pull images from Docker Hub, run and manage containers, map ports, and verify a containerized web server. I also learned the basic differences between virtual machines and containers and how containers can be useful for web application deployment.

## Challenges Encountered

One challenge I encountered was managing the Docker container and making sure that the correct commands were executed in the proper order. I also encountered some difficulty when organizing and uploading the required screenshots to the correct folder in GitHub. These challenges helped me become more familiar with Docker and GitHub repository management.
