# Simplified-Docker-Commands-with-examples
Explanation of each Docker Command

Simplified examples for the Docker commands you provided:

### 1. `docker run` - Run a container from an image
   - **Example:** 
     ```bash
     docker run -d --name my_container nginx
     ```
   - **Explanation:**
     - `-d`: Run the container in the background (detached mode).
     - `--name my_container`: Assign the name "my_container" to the running container.
     - `nginx`: Use the "nginx" image.

### 2. `docker pull` - Pull an image from a registry
   - **Example:** 
     ```bash
     docker pull ubuntu:latest
     ```
   - **Explanation:**
     - Pulls the latest version of the Ubuntu image from the default registry.

### 3. `docker push` - Push an image to a registry
   - **Example:** 
     ```bash
     docker push my_username/my_image:tag
     ```
   - **Explanation:**
     - Pushes the local image with the specified tag to a remote registry under the specified username.

### 4. `docker build` - Build an image from a Dockerfile
   - **Example:** 
     ```bash
     docker build -t my_image:tag .
     ```
   - **Explanation:**
     - `-t my_image:tag`: Tags the built image with the name "my_image" and the specified tag.
     - `.`: Specifies the build context as the current directory containing the Dockerfile.

### 5. `docker ps` - List running containers
   - **Example:** 
     ```bash
     docker ps
     ```
   - **Explanation:**
     - Lists the currently running containers.

### 6. `docker stop` - Stop a running container
   - **Example:** 
     ```bash
     docker stop my_container
     ```
   - **Explanation:**
     - Stops the running container named "my_container".

### 7. `docker start` - Start a stopped container
   - **Example:** 
     ```bash
     docker start my_container
     ```
   - **Explanation:**
     - Starts the stopped container named "my_container".

### 8. `docker restart` - Restart a container
   - **Example:** 
     ```bash
     docker restart my_container
     ```
   - **Explanation:**
     - Restarts the running or stopped container named "my_container".

### 9. `docker logs` - Show the logs of a container
   - **Example:** 
     ```bash
     docker logs my_container
     ```
   - **Explanation:**
     - Displays the logs of the container named "my_container".

### 10. `docker exec` - Execute a command inside a running container
   _ **Example:**
      ```bash
      docker exec -it my_container bash
      ```
    - **Explanation:**
      - `-it`: Opens an interactive terminal.
      - `bash`: Executes the Bash shell inside the running container named "my_container".

### 11. `docker images` - List available images
   - **Example:** 
      ```bash
      docker images
      ```
    - **Explanation:**
      - Lists the locally available Docker images.

### 12. `docker rm` - Remove a container
   - **Example:** 
      ```bash
      docker rm my_container
      ```
    - **Explanation:**
      - Removes the container named "my_container".

### 13. `docker rmi` - Remove an image
   - **Example:** 
      ```bash
      docker rmi my_image:tag
      ```
    - **Explanation:**
      - Removes the local image with the specified tag.

### 14. `docker inspect` - Show information about a container
   - **Example:** 
      ```bash
      docker inspect my_container
      ```
    - **Explanation:**
      - Displays detailed information about the container named "my_container".

### 15. `docker network create` - Create a network for containers to communicate
 - **Example:** 
      ```bash
      docker network create my_network
      ```
    - **Explanation:**
      - Creates a Docker network named "my_network" for containers to communicate.

### 16. `docker network connect` - Connect a container to a network
 - **Example:** 
      ```bash
      docker network connect my_network my_container
      ```
    - **Explanation:**
      - Connects the container named "my_container" to the "my_network" network.

### 17. `docker network disconnect` - Disconnect a container from a network
   - **Example:** 
      ```bash
      docker network disconnect my_network my_container
      ```
   **Explanation:**
      - Disconnects the container named "my_container" from the "my_network" network.

### 18. `docker port` - Show the mapped ports of a container
    - **Example:** 
      ```bash
      docker port my_container
      ```
   **Explanation:**
      - Displays the mapped ports of the container named "my_container".

### 19. `docker cp` - Copy files between a container and the host
    - **Example:** 
      ```bash
      docker cp my_container:/path/in/container /path/on/host
      ```
 - **Explanation:**
      - Copies files from the specified path in the container to the specified path on the host.

### 20. `docker commit` - Create a new image from a container's changes
    - **Example:** 
      ```bash

      docker commit my_container my_new_image:tag
      ```
   - **Explanation:**
      - Creates a new image named "my_new_image" with the specified tag from the changes made to the container named "my_container".

### 21. `docker login` - Log in to a registry
   - **Example:** 
     ```bash
     docker login myregistry.example.com
     ```
   - **Explanation:**
     - Logs in to the Docker registry at "myregistry.example.com".

### 22. `docker logout` - Log out of a registry
   - **Example:** 
     ```bash
     docker logout myregistry.example.com
     ```
   - **Explanation:**
     - Logs out of the Docker registry at "myregistry.example.com".

### 23. `docker tag` - Tag an image with a new name
   - **Example:** 
     ```bash
     docker tag my_image:tag myregistry.example.com/my_image:tag
     ```
   - **Explanation:**
     - Tags the local image with the specified tag with a new name in the format "myregistry.example.com/my_image:tag".

### 24. `docker export` - Export the contents of a container as a tar archive
   - **Example:** 
     ```bash
     docker export my_container > container-export.tar
     ```
   - **Explanation:**
     - Exports the contents of the container named "my_container" as a tar archive named "container-export.tar".

### 25. `docker import` - Create a new image from a tar archive
   - **Example:** 
     ```bash
     docker import container-export.tar my_new_image:tag
     ```
   - **Explanation:**
     - Creates a new image named "my_new_image" with the specified tag from a tar archive named "container-export.tar".

### 26. `docker save` - Save an image as a tar archive
   - **Example:** 
     ```bash
     docker save -o my_image.tar my_image:tag
     ```
   - **Explanation:**
     - Saves the image named "my_image" with the specified tag as a tar archive named "my_image.tar".

### 27. `docker load` - Load an image from a tar archive
   - **Example:** 
     ```bash
     docker load -i my_image.tar
     ```
   - **Explanation:**
     - Loads the image from the tar archive named "my_image.tar" into Docker.

### 28. `docker top` - Show the processes running inside a container
   - **Example:** 
     ```bash
     docker top my_container
     ```
   - **Explanation:**
     - Displays the processes running inside the container named "my_container".

### 29. `docker stats` - Show resource usage statistics of containers
   - **Example:** 
     ```bash
     docker stats
     ```
   - **Explanation:**
     - Displays real-time resource usage statistics of all running containers.

### 30. `docker diff` - Show the changes made to a container's filesystem
   - **Example:** 
     ```bash
     docker diff my_container
     ```
   - **Explanation:**
     - Shows the changes made to the filesystem of the container named "my_container".

### 31. `docker events` - Show the events generated by Docker
   - **Example:** 
     ```bash
     docker events
     ```
   - **Explanation:**
     - Displays real-time events generated by Docker.

### 32. `docker history` - Show the history of an image
   - **Example:** 
     ```bash
     docker history my_image:tag
     ```
   - **Explanation:**
     - Displays the history of the image named "my_image" with the specified tag.

### 33. `docker pause` - Pause a running container
   - **Example:** 
     ```bash
     docker pause my_container
     ```
   - **Explanation:**
     - Pauses the execution of the processes in the running container named "my_container".

### 34. `docker unpause` - Unpause a paused container
   - **Example:** 
     ```bash
     docker unpause my_container
     ```
   - **Explanation:**
     - Resumes the execution of the processes in the paused container named "my_container".

### 35. `docker kill` - Send a signal to a container to stop it abruptly
   - **Example:** 
     ```bash
     docker kill -s SIGTERM my_container
     ```
   - **Explanation:**
     - Sends the SIGTERM signal to the running container named "my_container" to stop it gracefully.

### 36. `docker wait` - Wait for a container to exit and return its exit code
   - **Example:** 
     ```bash
     docker wait my_container
     ```
   - **Explanation:**
     - Waits for the container named "my_container" to exit and returns its exit code.

### 37. `docker attach` - Attach to a running container's console
   - **Example:** 
     ```bash
     docker attach my_container
     ```
   - **Explanation:**
     - Attaches to the console of the running container named "my_container".

### 38. `docker buildx` - Build and push multi-platform images
   - **Example:** 
     ```bash
     docker buildx build --platform linux/amd64,linux/arm64 -t my_image:tag .
     ```
   - **Explanation:**
     - Builds and pushes a multi-platform image using Buildx.

### 39. `

docker compose` - Manage multi-container applications with Docker Compose
   - **Example:** 
     ```bash
     docker-compose up -d
     ```
   - **Explanation:**
     - Manages multi-container applications defined in a `docker-compose.yml` file, starting them in detached mode.

### 40. `docker swarm` - Create and manage a cluster of Docker nodes
   - **Example:** 
     ```bash
     docker swarm init
     ```
   - **Explanation:**
     - Initializes a Docker swarm to create and manage a cluster of Docker nodes.

### 41. `docker volume create` - Create a named volume for persistent data storage
   - **Example:** 
     ```bash
     docker volume create my_volume
     ```
   - **Explanation:**
     - Creates a named volume named "my_volume" for persistent data storage.

### 42. `docker volume ls` - List available volumes
   - **Example:** 
     ```bash
     docker volume ls
     ```
   - **Explanation:**
     - Lists the available Docker volumes.

### 43. `docker volume rm` - Remove a named volume
   - **Example:** 
     ```bash
     docker volume rm my_volume
     ```
   - **Explanation:**
     - Removes the named volume named "my_volume".

### 44. `docker system prune` - Remove all unused objects from Docker
   - **Example:** 
     ```bash
     docker system prune
     ```
   - **Explanation:**
     - Removes all unused Docker objects, including containers, networks, images, and volumes.

### 45. `docker system df` - Show the usage of Docker objects
   - **Example:** 
     ```bash
     docker system df
     ```
   - **Explanation:**
     - Displays the disk usage of Docker objects.

### 46. `docker system events` - Show the events generated by Docker on the system
   - **Example:** 
     ```bash
     docker system events
     ```
   - **Explanation:**
     - Displays real-time events generated by Docker on the system.

### 47. `docker system info` - Show system-wide information about Docker
   - **Example:** 
     ```bash
     docker system info
     ```
   - **Explanation:**
     - Displays system-wide information about Docker.

### 48. `docker system inspect` - Show detailed information about Docker objects
   - **Example:** 
     ```bash
     docker system inspect my_container
     ```
   - **Explanation:**
     - Displays detailed information about the Docker object named "my_container".

### 49. `docker system logs` - Show the system logs of Docker
   - **Example:** 
     ```bash
     docker system logs
     ```
   - **Explanation:**
     - Displays the system logs of Docker.

### 50. `docker system version` - Show the version of Docker installed on the system
   - **Example:** 
     ```bash
     docker system version
     ```
   - **Explanation:**
     - Displays the version of Docker installed on the system.

### 51. `docker exec` - Execute a command inside a running container
   - **Example:** 
     ```bash
     docker exec -it my_container ls /path/in/container
     ```
   - **Explanation:**
     - Executes the `ls` command inside the running container named "my_container" to list files in the specified path.

### 52. `docker inspect` - Show detailed information about Docker objects
   - **Example:** 
     ```bash
     docker inspect my_container
     ```
   - **Explanation:**
     - Displays detailed information about the Docker object named "my_container".

### 53. `docker network create` - Create a network for containers to communicate
   - **Example:** 
     ```bash
     docker network create my_network
     ```
   - **Explanation:**
     - Creates a Docker network named "my_network" for containers to communicate.

### 54. `docker network connect` - Connect a container to a network
   - **Example:** 
     ```bash
     docker network connect my_network my_container
     ```
   - **Explanation:**
     - Connects the container named "my_container" to the "my_network" network.

### 55. `docker network disconnect` - Disconnect a container from a network
   - **Example:** 
     ```bash
     docker network disconnect my_network my_container
     ```
   - **Explanation:**
     - Disconnects the container named "my_container" from the "my_network" network.

### 56. `docker port` - Show the mapped ports of a container
   - **Example:** 
     ```bash
     docker port my_container
     ```
   - **Explanation:**
     - Displays the mapped ports of the container named "my_container".

### 57. `docker cp` - Copy files between a container and the host
   - **Example:** 
     ```bash
     docker cp my_container:/path/in/container /path/on/host
     ```
   - **Explanation:**
     - Copies files from the specified path in the container to the specified path on the host.

### 58. `docker commit` - Create a new image from a container's changes
   - **Example:** 
     ```bash
     docker commit my_container my_new_image:tag
     ```
   - **Explanation:**
     - Creates a new image named "my_new_image" with the specified tag from the changes made to the container named "my_container".

### 59. `docker login` - Log in to a registry
   - **Example:** 
     ```bash
     docker login myregistry.example.com
     ```
   - **Explanation:**
     - Logs in to the Docker registry at "myregistry.example.com".

### 60. `docker logout` - Log out of a registry
   - **Example:** 
     ```bash
     docker logout myregistry.example.com
     ```
   - **Explanation:**
     - Logs out of the Docker registry at "myregistry.example.com".

### 61. `docker tag` - Tag an image with a new name
   - **Example:** 
     ```bash
     docker tag my_image:tag myregistry.example.com/my_image:tag
     ```
   - **Explanation:**
     - Tags the local image with the specified tag with a new name in the format "myregistry.example.com/my_image:tag".

### 62. `docker export` - Export the contents of a container as a tar archive
   - **Example:** 
     ```bash
     docker export my_container > container-export.tar
     ```
   - **Explanation:**
     - Exports the contents of the container named "my_container" as a tar archive named "container-export.tar".

### 63. `docker import` - Create a new image from a tar archive
   - **Example:** 
     ```bash
     docker import container-export.tar my_new_image:tag
     ```
   - **Explanation:**
     - Creates a new image named "my_new_image" with the specified tag from a tar archive named "container-export.tar".

### 64. `docker save` - Save an image as a tar archive
   - **Example:** 
     ```bash
     docker save -o my_image.tar my_image:tag
     ```
   - **Explanation:**
     - Saves the image named "my_image" with the specified tag as a tar archive named "my_image.tar".

### 65. `docker load` - Load an image from a tar archive
   - **Example:** 
     ```bash
     docker load -i my_image.tar
     ```
   - **Explanation:**
     - Loads the image from the tar archive named "my_image.tar" into Docker.

### 66. `docker top` - Show the processes running inside a container
   - **Example:** 
     ```bash
     docker top my_container
     ```
   - **Explanation:**
     - Displays the processes running inside the container named "my_container".

### 67. `docker stats` - Show resource usage statistics of containers


   - **Example:** 
     ```bash
     docker stats
     ```
   - **Explanation:**
     - Displays real-time resource usage statistics of all running containers.

### 68. `docker diff` - Show the changes made to a container's filesystem
   - **Example:** 
     ```bash
     docker diff my_container
     ```
   - **Explanation:**
     - Shows the changes made to the filesystem of the container named "my_container".

### 69. `docker events` - Show the events generated by Docker
   - **Example:** 
     ```bash
     docker events
     ```
   - **Explanation:**
     - Displays real-time events generated by Docker.

### 70. `docker history` - Show the history of an image
   - **Example:** 
     ```bash
     docker history my_image:tag
     ```
   - **Explanation:**
     - Displays the history of the image named "my_image" with the specified tag.

### 71. `docker pause` - Pause a running container
   - **Example:** 
     ```bash
     docker pause my_container
     ```
   - **Explanation:**
     - Pauses the execution of processes in the running container named "my_container".

### 72. `docker unpause` - Unpause a paused container
   - **Example:** 
     ```bash
     docker unpause my_container
     ```
   - **Explanation:**
     - Resumes the execution of processes in the paused container named "my_container".

### 73. `docker kill` - Send a signal to a container to stop it abruptly
   - **Example:** 
     ```bash
     docker kill -s SIGTERM my_container
     ```
   - **Explanation:**
     - Sends a specified signal (SIGTERM in this case) to the running container named "my_container" to stop it abruptly.

### 74. `docker wait` - Wait for a container to exit and return its exit code
   - **Example:** 
     ```bash
     docker wait my_container
     ```
   - **Explanation:**
     - Waits for the container named "my_container" to exit and then returns its exit code.

### 75. `docker attach` - Attach to a running container's console
   - **Example:** 
     ```bash
     docker attach my_container
     ```
   - **Explanation:**
     - Attaches to the console of the running container named "my_container," allowing interaction with its processes.

### 76. `docker buildx` - Build and push multi-platform images
   - **Example:** 
     ```bash
     docker buildx build --platform linux/amd64,linux/arm64 -t my_image:multi-platform .
     ```
   - **Explanation:**
     - Builds a multi-platform image for both AMD64 and ARM64 architectures and tags it as "my_image:multi-platform".

### 77. `docker compose` - Manage multi-container applications with Docker Compose
   - **Example:** 
     ```bash
     docker-compose up -d
     ```
   - **Explanation:**
     - Manages multi-container applications defined in a `docker-compose.yml` file, starting them in detached mode.

### 78. `docker swarm` - Create and manage a cluster of Docker nodes
   - **Example:** 
     ```bash
     docker swarm init
     ```
   - **Explanation:**
     - Initializes a Docker swarm to create and manage a cluster of Docker nodes.

### 79. `docker volume create` - Create a named volume for persistent data storage
   - **Example:** 
     ```bash
     docker volume create my_volume
     ```
   - **Explanation:**
     - Creates a named volume named "my_volume" for persistent data storage.

### 80. `docker volume ls` - List available volumes
   - **Example:** 
     ```bash
     docker volume ls
     ```
   - **Explanation:**
     - Lists the available Docker volumes.

### 81. `docker volume rm` - Remove a named volume
   - **Example:** 
     ```bash
     docker volume rm my_volume
     ```
   - **Explanation:**
     - Removes the named volume named "my_volume".

### 82. `docker system prune` - Remove all unused objects from Docker
   - **Example:** 
     ```bash
     docker system prune
     ```
   - **Explanation:**
     - Removes all unused Docker objects, including containers, networks, images, and volumes.

### 83. `docker system df` - Show the usage of Docker objects
   - **Example:** 
     ```bash
     docker system df
     ```
   - **Explanation:**
     - Displays the disk usage of Docker objects.

### 84. `docker system events` - Show the events generated by Docker on the system
   - **Example:** 
     ```bash
     docker system events
     ```
   - **Explanation:**
     - Displays real-time events generated by Docker on the system.

### 85. `docker system info` - Show system-wide information about Docker
   - **Example:** 
     ```bash
     docker system info
     ```
   - **Explanation:**
     - Displays system-wide information about Docker.

### 86. `docker system inspect` - Show detailed information about Docker objects
   - **Example:** 
     ```bash
     docker system inspect my_container
     ```
   - **Explanation:**
     - Displays detailed information about the Docker object named "my_container".

### 87. `docker system logs` - Show the system logs of Docker
   - **Example:** 
     ```bash
     docker system logs
     ```
   - **Explanation:**
     - Displays the system logs of Docker.

### 88. `docker system version` - Show the version of Docker installed on the system
   - **Example:** 
     ```bash
     docker system version
     ```
   - **Explanation:**
     - Displays the version of Docker installed on the system.

### 89. `docker pull` - Pull an image from a registry
   - **Example:** 
     ```bash
     docker pull myregistry.example.com/my_image:tag
     ```
   - **Explanation:**
     - Pulls the specified image with the given tag from the Docker registry at "myregistry.example.com" to the local machine.

### 90. `docker push` - Push an image to a registry
   - **Example:** 
     ```bash
     docker push my_image:tag
     ```
   - **Explanation:**
     - Pushes the locally built image with the specified tag to the default Docker registry.

### 91. `docker rm` - Remove a container
   - **Example:** 
     ```bash
     docker rm my_container
     ```
   - **Explanation:**
     - Removes the specified container named "my_container."

### 92. `docker rmi` - Remove an image
   - **Example:** 
     ```bash
     docker rmi my_image:tag
     ```
   - **Explanation:**
     - Removes the specified image with the given tag from the local machine.

### 93. `docker inspect` - Show detailed information about Docker objects
   - **Example:** 
     ```bash
     docker inspect my_image:tag
     ```
   - **Explanation:**
     - Displays detailed information about the Docker object, in this case, the image named "my_image" with the specified tag.

### 94. `docker network create` - Create a network for containers to communicate
   - **Example:** 
     ```bash
     docker network create my_network
     ```
   - **Explanation:**
     - Creates a Docker network named "my_network" for containers to communicate.

### 95. `docker network connect` - Connect a container to a network
   - **Example:** 
     ```bash
     docker network connect my_network my_container
     ```
   - **Explanation:**
     - Connects the container named "my_container" to the "my_network" network.

### 96. `docker network disconnect` - Disconnect a container from a network
   - **Example:** 
     ```bash
     docker network disconnect my_network my_container
     ```
   - **Explanation:**
     - Disconnects the container named "my_container" from the "my_network" network.

### 97. `docker port` - Show the mapped ports of a container
   - **Example:** 
     ```bash
     docker port my_container
     ```
   - **Explanation:**
     - Displays the mapped ports of the container named "my_container."

### 98. `docker cp` - Copy files between a container and the host
   - **Example:** 
     ```bash
     docker cp my_container:/path/in/container /path/on/host
     ```
   - **Explanation:**
     - Copies files from the specified path in the container to the specified path on the host.

### 99. `docker commit` - Create a new image from a container's changes
   - **Example:** 
     ```bash
     docker commit my_container my_new_image:tag
     ```
   - **Explanation:**
     - Creates a new image named "my_new_image" with the specified tag from the changes made to the container named "my_container."

### 100. `docker login` - Log in to a registry
   - **Example:** 
     ```bash
     docker login myregistry.example.com
     ```
   - **Explanation:**
     - Logs in to the Docker registry at "myregistry.example.com."

### 101. `docker logout` - Log out of a registry
   - **Example:** 
     ```bash
     docker logout myregistry.example.com
     ```
   - **Explanation:**
     - Logs out of the Docker registry at "myregistry.example.com."

### 102. `docker tag` - Tag an image with a new name
   - **Example:** 
     ```bash
     docker tag my_image:tag myregistry.example.com/my_image:tag
     ```
   - **Explanation:**
     - Tags the local image with the specified tag as "myregistry.example.com/my_image:tag" for pushing to a registry.

### 103. `docker export` - Export the contents of a container as a tar archive
   - **Example:** 
     ```bash
     docker export my_container > my_container_backup.tar
     ```
   - **Explanation:**
     - Exports the contents of the container named "my_container" as a tar archive to "my_container_backup.tar."

### 104. `docker import` - Create a new image from a tar archive
   - **Example:** 
     ```bash
     docker import my_container_backup.tar my_new_image:tag
     ```
   - **Explanation:**
     - Creates a new image named "my_new_image" with the specified tag from the contents of the tar archive.

### 105. `docker save` - Save an image as a tar archive
   - **Example:** 
     ```bash
     docker save -o my_image_backup.tar my_image:tag
     ```
   - **Explanation:**
     - Saves the image named "my_image" with the specified tag as a tar archive to "my_image_backup.tar."

### 106. `docker load` - Load an image from a tar archive
   - **Example:** 
     ```bash
     docker load -i my_image_backup.tar
     ```
   - **Explanation:**
     - Loads the image from the tar archive "my_image_backup.tar" into the local Docker images.

### 107. `docker top` - Show the processes running inside a container
   - **Example:** 
     ```bash
     docker top my_container
     ```
   - **Explanation:**
     - Displays the processes running inside the container named "my_container."

### 108. `docker stats` - Show resource usage statistics of containers
   - **Example:** 
     ```bash
     docker stats
     ```
   - **Explanation:**
     - Displays real-time resource usage statistics of all running containers.

### 109. `docker diff` - Show the changes made to a container's filesystem
   - **Example:** 
     ```bash
     docker diff my_container
     ```
   - **Explanation:**
     - Shows the changes made to the filesystem of the container named "my_container."

### 110. `docker events` - Show the events generated by Docker
   - **Example:** 
     ```bash
     docker events
     ```
   - **Explanation:**
     - Displays real-time events generated by Docker.

### 111. `docker history` - Show the history of an image
   - **Example:** 
     ```bash
     docker history my_image:tag
     ```
   - **Explanation:**
     - Displays the history of the image named "my_image" with the specified tag.

### 112. `docker pause` - Pause a running container
   - **Example:** 
     ```bash
     docker pause my_container
     ```
   - **Explanation:**
     - Pauses the execution of processes in the running container named "my_container."

### 113. `docker unpause` - Unpause a paused container
   - **Example:** 
     ```bash
     docker unpause my_container
     ```
   - **Explanation:**
     - Resumes the execution of processes in the paused container named "my_container."

### 114. `docker kill` - Send a signal to a container to stop it abruptly
   - **Example:** 
     ```bash
     docker kill -s SIGTERM my_container
     ```
   - **Explanation:**
     - Sends a specified signal (SIGTERM in this case) to the running container named "my_container" to stop it abruptly.

### 115. `docker wait` - Wait for a container to exit and return its exit code
   - **Example:** 
     ```bash
     docker wait my_container
     ```
   - **Explanation:**
     - Waits for the container named "my_container" to exit and then returns its exit code.

### 116. `docker attach` - Attach to a running container's console
   - **Example:** 
     ```bash
     docker attach my_container
     ```
   - **Explanation:**
     - Attaches to the console of the running container named "my_container," allowing interaction with its processes.

### 117. `docker buildx` - Build and push multi-platform images
   - **Example:** 
     ```bash
     docker buildx build --platform linux/amd64,linux/arm64 -t my_image:multi-platform .
     ```
   - **Explanation:**
     - Builds a multi-platform image for both AMD64 and ARM64 architectures and tags it as "my_image:multi-platform."

### 118. `docker compose` - Manage multi-container applications with Docker Compose
   - **Example:** 
     ```bash
     docker-compose up -d
     ```
   - **Explanation:**
     - Manages multi-container applications defined in a `docker-compose.yml` file, starting them in detached mode.

### 119. `docker swarm` - Create and manage a cluster of Docker nodes
   - **Example:** 
     ```bash
     docker swarm init
     ```
   - **Explanation:**
     - Initializes a Docker swarm to create and manage a cluster of Docker nodes.

### 120. `docker volume create` - Create a named volume for persistent data storage
   - **Example:** 
     ```bash
     docker volume create my_volume
     ```
   - **Explanation:**
     - Creates a named volume named "my_volume" for persistent data storage.

### 121. `docker volume ls` - List available volumes
   - **Example:** 
     ```bash
     docker volume ls
     ```
   - **Explanation:**
     - Lists the available Docker volumes on the local machine.

### 122. `docker volume rm` - Remove a named volume
   - **Example:** 
     ```bash
     docker volume rm my_volume
     ```
   - **Explanation:**
     - Removes the named volume named "my_volume."

### 123. `docker system prune` - Remove all unused objects from Docker
   - **Example:** 
     ```bash
     docker system prune
     ```
   - **Explanation:**
     - Removes all unused containers, networks, and volumes, freeing up disk space.

### 124. `docker system df` - Show the usage of Docker objects
   - **Example:** 
     ```bash
     docker system df
     ```
   - **Explanation:**
     - Displays the disk usage of Docker objects, including images, containers, and volumes.

### 125. `docker system events` - Show the events generated by Docker on the system
   - **Example:** 
     ```bash
     docker system events
     ```
   - **Explanation:**
     - Shows the system-wide events generated by Docker.

### 126. `docker system info` - Show system-wide information about Docker
   - **Example:** 
     ```bash
     docker system info
     ```
   - **Explanation:**
     - Displays system-wide information about the Docker installation.

### 127. `docker system inspect` - Show detailed information about Docker objects
   - **Example:** 
     ```bash
     docker system inspect my_image:tag
     ```
   - **Explanation:**
     - Displays detailed information about the specified Docker object, such as an image.

### 128. `docker system logs` - Show the system logs of Docker
   - **Example:** 
     ```bash
     docker system logs
     ```
   - **Explanation:**
     - Displays the system logs of Docker, including informational and error messages.

### 129. `docker system version` - Show the version of Docker installed on the system
   - **Example:** 
     ```bash
     docker system version
     ```
   - **Explanation:**
     - Displays the version of Docker installed on the system.

### 130. `docker plugin` - Manage Docker plugins
   - **Example:** 
     ```bash
     docker plugin install my_plugin
     ```
   - **Explanation:**
     - Installs a Docker plugin named "my_plugin."

### 131. `docker system prune -a` - Remove all unused objects, including images
   - **Example:** 
     ```bash
     docker system prune -a
     ```
   - **Explanation:**
     - Removes all unused containers, networks, volumes, and images, freeing up disk space.

### 132. `docker info` - Display system-wide information
   - **Example:** 
     ```bash
     docker info
     ```
   - **Explanation:**
     - Displays detailed information about the Docker system.

### 133. `docker version` - Show the Docker version information
   - **Example:** 
     ```bash
     docker version
     ```
   - **Explanation:**
     - Displays the version information for the Docker client and server.

### 134. `docker search` - Search for Docker images on Docker Hub
   - **Example:** 
     ```bash
     docker search ubuntu
     ```
   - **Explanation:**
     - Searches for Docker images related to "ubuntu" on Docker Hub.

### 135. `docker events` - Monitor Docker events in real-time
   - **Example:** 
     ```bash
     docker events --filter 'event=start'
     ```
   - **Explanation:**
     - Monitors Docker events in real-time, filtering for events where containers start.

### 136. `docker save` - Save multiple images as a tar archive
   - **Example:** 
     ```bash
     docker save -o my_images_backup.tar image1:tag image2:tag
     ```
   - **Explanation:**
     - Saves multiple images as a tar archive named "my_images_backup.tar."

### 137. `docker load` - Load multiple images from a tar archive
   - **Example:** 
     ```bash
     docker load -i my_images_backup.tar
     ```
   - **Explanation:**
     - Loads multiple images from the tar archive "my_images_backup.tar" into the local Docker images.

### 138. `docker ps -a` - List all containers, including stopped ones
   - **Example:** 
     ```bash
     docker ps -a
     ```
   - **Explanation:**
     - Lists all containers, including both running and stopped ones.

### 139. `docker stats` - Show resource usage statistics of specific containers
   - **Example:** 
     ```bash
     docker stats container1 container2
     ```
   - **Explanation:**
     - Displays real-time resource usage statistics for specific containers.

### 140. `docker history` - Show the history of multiple images
   - **Example:** 
     ```bash
     docker history image1:tag image2:tag
     ```
   - **Explanation:**
     - Displays the history of multiple Docker images.

### 141. `docker port` - Show the mapped ports of a running container
   - **Example:** 
     ```bash
     docker port my_container
     ```
   - **Explanation:**
     - Displays the mapped ports of the running container named "my_container."

### 142. `docker cp` - Copy files between a container and the host
   - **Example:** 
     ```bash
     docker cp my_container:/path/in/container /path/on/host
     ```
   - **Explanation:**
     - Copies files from the specified path in the container to the specified path on the host.

### 143. `docker commit` - Create a new image from a container's changes
   - **Example:** 
     ```bash
     docker commit my_container my_new_image:tag
     ```
   - **Explanation:**
     - Creates a new image named "my_new_image" with the specified tag from the changes made in the container.

### 144. `docker attach` - Attach to a running container's console
   - **Example:** 
     ```bash
     docker attach my_container
     ```
   - **Explanation:**
     - Attaches to the console of the running container named "my_container," allowing interaction with its processes.

### 145. `docker buildx` - Build and push multi-platform images
   - **Example:** 
     ```bash
     docker buildx create --use
     ```
   - **Explanation:**
     - Creates a new builder instance and sets it as the active builder for building multi-platform images.

### 146. `docker-compose` - Manage multi-container applications with Docker Compose
   - **Example:** 
     ```bash
     docker-compose up -d
     ```
   - **Explanation:**
     - Manages multi-container applications defined in a `docker-compose.yml` file, starting them in detached mode.

### 147. `docker swarm` - Create and manage a cluster of Docker nodes
   - **Example:** 
     ```bash
     docker swarm init
     ```
   - **Explanation:**
     - Initializes a Docker swarm to create and manage a cluster of Docker nodes.

### 148. `docker network create` - Create a network for containers to communicate
   - **Example:** 
     ```bash
     docker network create my_network
     ```
   - **Explanation:**
     - Creates a Docker network named "my_network" for containers to communicate with each other.

### 149. `docker network connect` - Connect a container to a network
   - **Example:** 
     ```bash
     docker network connect my_network my_container
     ```
   - **Explanation:**
     - Connects the container named "my_container" to the Docker network named "my_network."

### 150. `docker network disconnect` - Disconnect a container from a network
   - **Example:** 
     ```bash
     docker network disconnect my_network my_container
     ```
   - **Explanation:**
     - Disconnects the container named "my_container" from the Docker network named "my_network."

### 151. `docker exec` - Execute a command inside a running container
   - **Example:** 
     ```bash
     docker exec -it my_container bash
     ```
   - **Explanation:**
     - Executes an interactive bash session inside the running container named "my_container."

### 152. `docker export` - Export the contents of a container as a tar archive
   - **Example:** 
     ```bash
     docker export my_container > container_backup.tar
     ```
   - **Explanation:**
     - Exports the contents of the running container named "my_container" as a tar archive named "container_backup.tar."

### 153. `docker import` - Create a new image from a tar archive
   - **Example:** 
     ```bash
     docker import my_image.tar my_new_image:tag
     ```
   - **Explanation:**
     - Creates a new Docker image named "my_new_image" with the specified tag from a tar archive named "my_image.tar."

### 154. `docker wait` - Wait for a container to exit and return its exit code
   - **Example:** 
     ```bash
     docker wait my_container
     ```
   - **Explanation:**
     - Waits for the specified container ("my_container") to exit and returns its exit code.

### 155. `docker kill` - Send a signal to a container to stop it abruptly
   - **Example:** 
     ```bash
     docker kill -s SIGTERM my_container
     ```
   - **Explanation:**
     - Sends the SIGTERM signal to the running container named "my_container" to stop it gracefully.

### 156. `docker pause` - Pause a running container
   - **Example:** 
     ```bash
     docker pause my_container
     ```
   - **Explanation:**
     - Pauses the execution of processes in the running container named "my_container."

### 157. `docker unpause` - Unpause a paused container
   - **Example:** 
     ```bash
     docker unpause my_container
     ```
   - **Explanation:**
     - Resumes the execution of processes in a paused container named "my_container."

### 158. `docker top` - Show the processes running inside a container
   - **Example:** 
     ```bash
     docker top my_container
     ```
   - **Explanation:**
     - Displays the processes running inside the container named "my_container."

### 159. `docker diff` - Show the changes made to a container's filesystem
   - **Example:** 
     ```bash
     docker diff my_container
     ```
   - **Explanation:**
     - Displays the changes made to the filesystem of the running container named "my_container."

### 160. `docker system logs` - Show the system logs of Docker
   - **Example:** 
     ```bash
     docker system logs
     ```
   - **Explanation:**
     - Displays the system logs of Docker, including informational and error messages.

### 161. `docker attach` - Attach to a running container's console
   - **Example:** 
     ```bash
     docker attach my_container
     ```
   - **Explanation:**
     - Attaches to the console of the running container named "my_container," allowing interaction with its processes.

### 162. `docker swarm` - Create and manage a cluster of Docker nodes
   - **Example:** 
     ```bash
     docker swarm init
     ```
   - **Explanation:**
     - Initializes a Docker swarm to create and manage a cluster of Docker nodes.

### 163. `docker swarm join` - Join a Docker node to a swarm
   - **Example:** 
     ```bash
     docker swarm join --token <swarm-token> <swarm-manager-ip>
     ```
   - **Explanation:**
     - Joins a Docker node to an existing swarm using the provided token and swarm manager IP.

### 164. `docker swarm leave` - Leave a Docker swarm
   - **Example:** 
     ```bash
     docker swarm leave
     ```
   - **Explanation:**
     - Makes a Docker node leave the swarm it is currently part of.

### 165. `docker service` - Manage Docker services
   - **Example:** 
     ```bash
     docker service create --replicas 3 my_image
     ```
   - **Explanation:**
     - Creates a Docker service with three replicas using the specified image.

### 166. `docker stack` - Deploy a Docker stack
   - **Example:** 
     ```bash
     docker stack deploy -c docker-compose.yml my_stack
     ```
   - **Explanation:**
     - Deploys a Docker stack using the services defined in the provided `docker-compose.yml` file.

### 167. `docker node` - Manage Docker nodes
   - **Example:** 
     ```bash
     docker node ls
     ```
   - **Explanation:**
     - Lists the Docker nodes in the swarm.

### 168. `docker secret` - Manage Docker secrets
   - **Example:** 
     ```bash
     echo "my_secret_data" | docker secret create my_secret -
     ```
   - **Explanation:**
     - Creates a Docker secret named "my_secret" from the provided data.

### 169. `docker config` - Manage Docker configs
   - **Example:** 
     ```bash
     echo "my_config_data" | docker config create my_config -
     ```
   - **Explanation:**
     - Creates a Docker config named "my_config" from the provided data.

### 170. `docker plugin` - Manage Docker plugins
   - **Example:** 
     ```bash
     docker plugin install my_plugin
     ```
   - **Explanation:**
     - Installs a Docker plugin named "my_plugin."

### 171. `docker image prune` - Remove unused images
   - **Example:** 
     ```bash
     docker image prune
     ```
   - **Explanation:**
     - Removes unused Docker images, freeing up disk space.

### 172. `docker container prune` - Remove stopped containers
   - **Example:** 
     ```bash
     docker container prune
     ```
   - **Explanation:**
     - Removes all stopped containers, freeing up resources.

### 173. `docker volume prune` - Remove unused volumes
   - **Example:** 
     ```bash
     docker volume prune
     ```
   - **Explanation:**
     - Removes unused Docker volumes, freeing up disk space.

### 174. `docker network prune` - Remove unused networks
   - **Example:** 
     ```bash
     docker network prune
     ```
   - **Explanation:**
     - Removes unused Docker networks, freeing up resources.

### 175. `docker system prune -a` - Remove all unused objects, including images
   - **Example:** 
     ```bash
     docker system prune -a
     ```
   - **Explanation:**
     - Removes all unused containers, networks, volumes, and images, freeing up disk space.

### 176. `docker system df` - Show the usage of Docker objects
   - **Example:** 
     ```bash
     docker system df
     ```
   - **Explanation:**
     - Displays the disk usage of Docker objects, including containers, images, and volumes.

### 177. `docker system events` - Show the events generated by Docker on the system
   - **Example:** 
     ```bash
     docker system events
     ```
   - **Explanation:**
     - Displays real-time events generated by Docker on the system.

### 178. `docker system inspect` - Show detailed information about Docker objects
   - **Example:** 
     ```bash
     docker system inspect
     ```
   - **Explanation:**
     - Displays detailed information about Docker objects, including containers, images, volumes, and networks.

### 179. `docker system logs` - Show the system logs of Docker
   - **Example:** 
     ```bash
     docker system logs
     ```
   - **Explanation:**
     - Displays the system logs of Docker, including informational and error messages.

### 180. `docker system version` - Show the version of Docker installed on the system
   - **Example:** 
     ```bash
     docker system version
     ```
   - **Explanation:**
     - Displays the version information for Docker installed on the system.

These examples cover various Docker system-related commands for managing resources, cleaning up unused objects, and inspecting system information.
