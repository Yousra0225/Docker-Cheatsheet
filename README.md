# Docker Documentation

- [What is Docker ?](#docker-documentation)
- [Docker Idea](#docker-idea)
- [Docker Container](#container-history)
- [Virtual Machine](#container-history)
- [Docker Commannds](#container-history)
- [Docker Properties](#container-history)
- [Docker Images](#container-history)
- [Docker Volumes](#container-history)
- [Docker Networks](#container-history)
- [Docker Hub](#container-history)
- [Images Layers](#container-history)
- [Cross Container](#container-history)
- [Projects](#container-history)
- [Docker Composer](#container-history)

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

### Dockerfile 

|Term|Explanation|
|----|-----------|
|`From`|Define the base image that contains a minimal filesystem and environment, on top of which we add additional files and configurations.|
|`COPY`|copies files or directories from the build context (your local machine) into the container’s filesystem at a specified path.|
|`WORKDIR`|defines the working directory inside the container where subsequent commands will be executed.|
|`CMD`|specifies the default command and arguments that will run when a container it started from image|



