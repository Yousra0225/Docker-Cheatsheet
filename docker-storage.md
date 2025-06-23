# 🐳 Docker Storage

## Volume mounts

- A volume is a way to store data in Docker.
- It keeps data even if the container is deleted.
- The data is saved on the host of the computer.

## Volumes Commands

| Command                             | Description                        |
| ----------------------------------- | ---------------------------------- |
| `docker volume create` volume-name  | Create a Docker volume             |
| `docker volume inspect` volume-name | Show the volume details            |
| `docker volume ls`                  | Lists all volumes                  |
| `docker rm ` volume-name            | Deletes the volume                 |
| `docker run -v` volume-name         | Mounts a volume into the container |
| `docker run --mount`                | Alternative way to mount a volume  |
