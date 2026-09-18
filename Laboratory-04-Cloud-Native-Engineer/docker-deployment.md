# Docker Deployment

## Nginx Deployment

### Pull the Nginx Image

```bash
docker pull nginx
```

This downloads the official Nginx image from Docker Hub to the local Docker environment.

### Run the Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

This starts an Nginx container in detached mode and maps port 8080 on the host to port 80 inside the container.

### Check the Running Container

```bash
docker ps
```

This displays the containers that are currently running.

### Test the Web Server

```bash
curl http://localhost:8080
```

This sends a local HTTP request to the Nginx server and displays the response in the terminal.

## Container Lifecycle

### List Running Containers

```bash
docker ps
```

This shows the containers that are currently running.

### Stop the Container

```bash
docker stop nginx-server
```

This stops the running Nginx container.

### Verify the Container Is Stopped

```bash
docker ps
```

This confirms that the Nginx container is no longer running.

### Check All Containers

```bash
docker ps -a
```

This shows both running and stopped containers, allowing the stopped Nginx container to be verified.

### Remove the Container

```bash
docker rm nginx-server
```

This permanently removes the stopped Nginx container from the Docker environment.

## Screenshot Evidence

The container lifecycle commands were executed in the KillerCoda terminal. The screenshot is saved as:

`screenshots/container-lifecycle.png`
