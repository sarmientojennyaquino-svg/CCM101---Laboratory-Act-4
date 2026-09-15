# Docker Container Lifecycle

## 1. List Running Containers

```bash
docker ps
```

This command lists the Docker containers that are currently running.

## 2. Stop the Running Container

```bash
docker stop nginx-server
```

This command stops the running `nginx-server` container.

## 3. Verify the Container Is Stopped

```bash
docker ps
```

This command verifies that the `nginx-server` container is no longer running.

To view stopped containers, the following command can also be used:

```bash
docker ps -a
```

## 4. Remove the Container Completely

```bash
docker rm nginx-server
```

This command permanently removes the stopped `nginx-server` container.
