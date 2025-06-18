# Dockerfile 
## Structure 
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