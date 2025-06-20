# 🐳 Docker Commands

## Docker Image

| Command                       | Description                                                |
| ----------------------------- | ---------------------------------------------------------- |
| `docker build -t name .`      | Build an image from a Dockerfile in the current directory. |
| `docker images`               | List all local Docker images.                              |
| `docker image ls`             | Same as `docker images`: list local images.                |
| `docker pull user/image-name` | Download an image from Docker Hub.                         |
| `docker push user/image-name` | Upload an image to Docker Hub.                             |
| `docker rmi image`            | Remove a local Docker image.                               |
| `docker tag image user/image` | Tag an image with a new name before pushing to Docker Hub. |

## Docker Container

| Command                          | Explanation                                                        |
| -------------------------------- | ------------------------------------------------------------------ |
| `docker run image`               | Create and start a container from an image.                        |
| `docker run -it image /bin/bash` | Create a container from an image and opens an interactive terminal |
| `docker exec -it container bash` | Start an interactive terminal session inside a running container.  |
| `docker logs container`          | Show logs from a container.                                        |
| `docker start container-id`      | Start th container                                                 |
| `docker stop container`          | Stop the container from runninf=g                                  |
| `docker ps`                      | List running containers only.                                      |
| `docker ps -a`                   | List all containers (running and stopped).                         |
| `docker stop container`          | Stop a running container.                                          |
| `docker rm container`            | Remove a stopped container.                                        |
| `docker info`                    | Show detailed info about Docker client and server.                 |
| `docker login`                   | Log in to Docker Hub from the terminal.                            |
