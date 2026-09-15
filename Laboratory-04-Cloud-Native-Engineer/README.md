# Laboratory 04 – The Cloud-Native Engineer

## Mission Overview

This laboratory activity introduced the basic concepts and practices of cloud-native engineering through containerization. The activity focused on understanding the differences between Virtual Machines and Containers and using Docker to deploy and manage an Nginx web server. The Docker Playground was used to pull an Nginx image, run a container, test the web server, and manage its lifecycle.

## Objectives

* Differentiate between traditional Virtual Machines and Containers.
* Access a Docker-enabled cloud environment using KillerCoda.
* Execute fundamental Docker CLI commands.
* Pull and run a containerized Nginx web server.
* Manage and terminate a Docker container.
* Document container operations using Markdown.
* Develop and organize a GitHub Cloud Computing portfolio.

## Docker Commands Executed

### Checkpoint 3 – Verify Docker

```bash
docker --version
docker info
```

### Checkpoint 4 – Deploy Nginx

```bash
docker pull nginx
docker run -d -p 8080:80 --name nginx-server nginx
curl http://localhost:8080
```

### Checkpoint 5 – Container Lifecycle

```bash
docker ps
docker stop nginx-server
docker ps
docker ps -a
docker rm nginx-server
docker ps -a
```

## Skills Learned

Through this laboratory activity, I learned how to use basic Docker commands in a Linux environment. I learned how to pull Docker images, create and run containers, map network ports, and verify a containerized web server using an HTTP request. I also learned how to stop, verify, and remove containers and document technical procedures using Markdown and GitHub.

## Challenges Encountered

One challenge was becoming familiar with the Docker command-line interface and understanding the purpose of each command. Another challenge was understanding port mapping and how the host port connects to the port used by the web server inside the container. Managing the container lifecycle also required careful execution of the commands in the correct order. These challenges helped improve my confidence in using Docker and working with containerized applications.
