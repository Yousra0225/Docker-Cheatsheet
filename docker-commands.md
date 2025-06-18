# 🐳 Docker Commands Cheatsheet

| Command                          | Description                                                         |
| -------------------------------- | ------------------------------------------------------------------- |
| `docker build -t name .`         | Build an image from a Dockerfile in the current directory.          |
| `docker exec -it container bash` | Start an interactive terminal session inside a running container.   |
| `docker images`                  | List all local Docker images.                                       |
| `docker image ls`                | Same as `docker images`: list local images.                         |
| `docker info`                    | Show detailed info about Docker client and server.                  |
| `docker login`                   | Log in to Docker Hub from the terminal.                             |
| `docker logs container`          | Show logs from a container.                                         |
| `docker ps`                      | List running containers only.                                       |
| `docker ps -a`                   | List all containers (running and stopped).                          |
| `docker pull user/image`         | Download an image from Docker Hub.                                  |
| `docker push user/image`         | Upload an image to Docker Hub.                                      |
| `docker rm container`            | Remove a stopped container.                                         |
| `docker rmi image`               | Remove a local Docker image.                                        |
| `docker run image`               | Create and start a container from an image.                         |
| `docker stop container`          | Stop a running container.                                           |
| `docker tag image user/image`    | Tag an image with a new name (useful before pushing to Docker Hub). |

-` Docker Compose` : Outil qui permet de définir et lancer plusieurs conteneurs Docker en même temps via un fichier YAML. 
- `Docker Swarm` :  Il transforme plusieurs hôtes Docker en un cluster unique, répartit automatiquement les conteneurs sur les nœuds
- 