## Docker Commands

Docker is a powerful tool for managing containers. Here are some of the main Docker commands:

## **docker run**: Create and start a new container from an image.
   docker run [options] [image] [command] [arguments]

### **docker pull**: Download an image from a container registry.
   docker pull [image]

### **docker build**: Build a Docker image from a Dockerfile.
   docker build [options] -t [image_name] [path]

### **docker images**: List all Docker images on your system.
   docker images

### **docker ps**:  List all running containers.
   docker ps

### **docker stop**:  Stop a running container.
   docker stop [container]

### **docker start**:  Start a stopped container.
   docker start [container]

### **docker restart**:  Restart a running or stopped container.
   docker restart [container]

### **docker rm**:  Remove a stopped container.
   docker rm [container]

### **docker rmi**:  Remove an image.
   docker rmi [image]

### **docker exec**:  Run a command in a running container.
   docker exec [options] [container] [command]

### **docker logs**:  View the logs of a container.
   docker logs [container]

### **docker network**:  Manage Docker networks for connecting containers.
    docker network [subcommand]