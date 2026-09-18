# Mission Reflection

## 1. Docker Containers vs. Virtual Machines

Docker containers are much faster to start and set up compared to installing an operating system on a Virtual Machine. A VM needs to boot a complete operating system, which can take several minutes and uses more system resources. A Docker container uses the host operating system kernel, so it can start within seconds. In this activity, I was able to pull and run an Nginx container quickly using only a few Docker commands.

## 2. Importance of Port Mapping

Port mapping such as `-p 8080:80` is necessary because the Nginx web server is running inside the container on port 80, while users access the service through the host machine. The mapping connects port 8080 of the host to port 80 inside the container. This allowed me to access the Nginx server using `curl http://localhost:8080`.

## 3. What Happens When a Container Is Removed

When `docker rm` is used, the container itself is permanently removed. Any data stored only inside the container that was not saved using a volume or another external storage method can also be lost. The Docker image, however, is separate from the container and can still be used to create a new container.

## 4. Containerization and DevOps

Containerization can make collaboration between developers and IT operations teams easier because applications can be packaged with their dependencies in a consistent environment. Developers can build and test containers while operations teams can deploy the same container in different environments. This can reduce differences between development and production environments and support faster deployment.

## 5. My GitHub Portfolio

My GitHub portfolio is gradually becoming a record of the cloud computing skills I have learned through different laboratory activities. In this mission, I added documentation about virtual machines, containers, Docker commands, Nginx deployment, and container lifecycle management. As I continue adding more laboratories, my portfolio shows my progress and practical experience in cloud computing.
