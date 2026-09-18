# Docker Container Lifecycle

## 1. List Running Containers

```bash
docker ps
```

This command lists all currently running Docker containers.

## 2. Stop the Running Container

```bash
docker stop my-nginx
```

This command stops the running `my-nginx` container.

## 3. Verify the Container is Stopped

```bash
docker ps
```

This command verifies that `my-nginx` is no longer running.

## 4. Remove the Container Completely

```bash
docker rm my-nginx
```

This command removes the stopped `my-nginx` container completely.
