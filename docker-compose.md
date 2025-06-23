# Docker Compose 
![Docker compose illustration](./src/Docker-Compose.png)  
*Tool for building and running multi-container applications with one command. It manages interaction and networking between containers and their ports.*  

## Basic docker-compose.yml example  
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

## Compose File properties 

### 1. Version
*Compose file version supported by the Docker Engine.*
```yml
version: "3.9"
```

### 2. Services 
*It's a definition of a Docker container configuration within the docker-compose.yml file. It specifies which Docker image to use, dockerfile location , and the container’s runtime settings (ports, volumes, environment variables, networks). Each service corresponds to one or more containers running the same configuration.*
```yml
services:
    frontend:
        build: ./web # Path to the Dockerfile for the frontend
        ports: 
            - <host_port>:<container_port>
    backend:
        build: ./api # Path to the Dockerfile for the api
        ports: 
            - <host_port>:<container_port>
    database:
        image: postgres:<version> # build the image for db
            - <host_port>:<container_port>
```