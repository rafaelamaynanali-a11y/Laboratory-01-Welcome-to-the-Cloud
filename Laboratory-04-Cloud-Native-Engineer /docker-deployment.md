# Docker Deployment & Container Lifecycle

## Nginx Deployment Commands

| Command | Explanation |
|---|---|
| `docker pull nginx` | Downloads the official Nginx web server image from Docker Hub to the local environment. |
| `docker run -d -p 8080:80 --name my-nginx nginx` | Creates and starts a new container in detached mode, maps host port 8080 to container port 80, and assigns the name "my-nginx". |
| `curl http://localhost:8080` | Sends an HTTP request to the locally exposed port to verify the web server is responding. |

## Container Lifecycle Commands

| Command | Explanation |
|---|---|
| `docker ps` | Lists all currently running containers with their status, ports, and names. |
| `docker stop my-nginx` | Gracefully stops the running container without immediately deleting it. |
| `docker ps -a` | Shows all containers including stopped ones to confirm the container is no longer running. |
| `docker rm my-nginx` | Permanently deletes the stopped container; it is removed entirely from the system. |
