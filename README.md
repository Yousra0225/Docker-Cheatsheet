# Docker Documentation

- [What is Docker ?](#docker-documentation)
- [Docker Idea](#docker-idea)
- [Docker Commannds](./docker-commands.md)
- [Docker Properties](#container-history)
- [Docker Images](#container-history)
- [Docker Container](#container-history)
- [Dockerfile](./docker-file.md)
- [Docker Volumes](#docker-compose)
- [Docker Compose](#DOCKER-COMPOSE)
- [Docker Networks](#container-history)
- [Docker Hub](#container-history)
- [Cross Container](#container-history)

## What is Docker ?

### Definition

Docker is an open plateform for developing, shipping, and running applications.
The main objectives of Docker :  

|||
| --------------------- | ----------------------------------------------------------------------- |
| **Portability** | Run the same application across different environments without changes. |
| **Isolation** | Separate applications and dependencies to avoid version conflicts. |
| **Lightweight and Fast** | Use fewer resources and start faster than virtual machines. |
| **Simplified Deployment**| Automate building, shipping, and running applications. |
| **Faster Delivery** | Reduce time between writing code and running it in production. |

### Docker Engine 
Docker Engine is the program you install on your machine that allows to build images, run containers, and manage container, images, networks ...

### Docker image 
Docker image is a snapshot of the complete environment needed for the app — including language versions, dependencies, libraries, and configurations.


### Docker Container 
Docker container is a instance/copy/object of/from image. executable

### Docker Compose
Tool for building and running multi-container applications with one command. It manages interaction and networking between containers and their ports.  
**Basic docker-compose.yml example**
```yaml
version: '3.8'

services:
  app:
    build: .
    ports:
      - "3000:3000"
    volumes:
      - .:/app
    depends_on:
      - db

  db:
    image: postgres:14
    environment:
      POSTGRES_USER: user
      POSTGRES_PASSWORD: pass
      POSTGRES_DB: mydb
    volumes:
      - pgdata:/var/lib/postgresql/data

volumes:
  pgdata:
```


