# Laboratory 04: The Cloud-Native Engineer

## Mission Overview

This laboratory activity introduced the basic concepts of cloud-native computing and containerization. I compared Virtual Machines and containers, then used the KillerCoda Docker environment to deploy an Nginx web server. I also practiced basic Docker commands for running, checking, stopping, and removing a container.

## Objectives

- Differentiate Virtual Machines from containers.
- Verify that Docker is installed and running in a Linux environment.
- Pull and run an Nginx Docker image.
- Use port mapping to access a web server inside a container.
- Manage the basic lifecycle of a Docker container.
- Document Docker commands and procedures using Markdown.

## Docker Commands Executed

### Check Docker Installation

```bash
docker --version
```

Used to check the installed Docker version.

### Check Docker Environment

```bash
docker info
```

Used to view information about the Docker client, server, containers, images, and system configuration.

### Pull Nginx

```bash
docker pull nginx
```

Downloads the Nginx image from Docker Hub.

### Run Nginx

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

Runs the Nginx container in detached mode and maps port 8080 on the host to port 80 inside the container.

### List Running Containers

```bash
docker ps
```

Displays the containers that are currently running.

### Test Nginx

```bash
curl http://localhost:8080
```

Sends an HTTP request to the Nginx web server through port 8080.

### Stop the Container

```bash
docker stop nginx-server
```

Stops the running Nginx container.

### Check All Containers

```bash
docker ps -a
```

Displays both running and stopped containers.

### Remove the Container

```bash
docker rm nginx-server
```

Removes the stopped Nginx container.

## Skills Learned

- Basic Docker CLI usage
- Container deployment
- Docker image management
- Port mapping
- Container lifecycle management
- Linux terminal commands
- Technical documentation using Markdown
- Organizing laboratory evidence in GitHub

## Challenges Encountered

One challenge was understanding the difference between a Docker image and a container. The image provides the files and configuration needed to create the application environment, while the container is the running instance of that image. I also had to understand how port mapping allows a service inside the container to be accessed through the host machine.

Another part that required attention was managing the container lifecycle. Stopping a container does not remove it, so `docker rm` is needed when the container is no longer needed.
