# Dockerfile

## Structure example

```dockerfile
# Step 1: Specify the base image
FROM node:18-alpine

# Step 2: Set the working directory inside the container
WORKDIR /app

# Step 3: Copy local files into the container
COPY . .

# Step 4: Install dependencies (if it's a Node.js project)
RUN npm install

# Step 5: Expose the application port
EXPOSE 3000

# Step 6: Specify the default command to run when the container starts
CMD npm
```
## Instructions 

| Instruction   | Explanation                                                      |
| ------------- | ---------------------------------------------------------------- |
| `FROM`        | Sets the base image (ex `FROM node:18-alpine`)                   |
| `WORKDIR`     | Sets the working directory inside the container                  |
| `COPY`        | Copies files from the computer into the container                |
| `ADD`         | Like `COPY`, but can also handle URLs and `.tar` archives        |
| `RUN`         | Runs a command while building the image (e.g. `RUN npm install`) |
| `CMD`         | Sets the default command to run when the container starts        |
| `ENTRYPOINT`  | Similar to `CMD`, but cannot be easily overridden                |
| `ENV`         | Sets an environment variable inside the container                |
| `EXPOSE`      | Tells Docker what port the app will use                          |
| `LABEL`       | Adds extra info (like author name or version) to the image       |
| `VOLUME`      | Creates a folder that can be shared with your computer           |
| `USER`        | Sets which user will run the next commands in the Dockerfile     |
| `ARG`         | Sets a variable only used during the build                       |
| `HEALTHCHECK` | Adds a check to see if your app is running properly              |
