# Mission Reflection

This laboratory activity helped me understand how containerization can make application deployment faster and more efficient. A Docker container can start in seconds because it shares the host operating system kernel, while a Virtual Machine needs to boot a complete operating system before the application can run. This makes containers useful when applications need to be deployed and started quickly.

The port mapping `-p 8080:80` is necessary because the Nginx web server is running inside the container on port 80, while port 8080 is exposed on the host machine. By mapping port 8080 on the host to port 80 inside the container, I was able to access the Nginx web server using `curl http://localhost:8080`. Without this mapping, the web server would not be directly accessible through the host's port 8080.

When `docker rm` is used, the specified container is removed from the Docker environment. Any data stored only inside the container can be lost when the container is removed, which shows why persistent data should be stored using appropriate storage such as volumes when it needs to survive the container lifecycle.

Containerization can also improve collaboration between software developers and IT operations teams. Developers can package an application and its dependencies into a container, while operations teams can run the same containerized application in different environments. This supports the DevOps approach by making deployment more consistent and repeatable.

Finally, my GitHub portfolio is evolving as I continue adding organized laboratory activities and technical documentation. Each laboratory gives me an opportunity to demonstrate what I have learned about cloud computing and document my practical experience. The portfolio is becoming a record of my progress and developing technical skills.
