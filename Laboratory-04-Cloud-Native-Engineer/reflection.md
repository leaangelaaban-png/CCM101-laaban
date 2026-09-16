# Mission Reflection

In this laboratory activity, I learned that Docker containers are much faster to start and set up compared to Virtual Machines. A Virtual Machine needs its own operating system, which takes more time to install and boot. A Docker container shares the host operating system, so it can start within seconds. This made me understand why containers are useful when applications need to be deployed quickly.

I also learned the purpose of port mapping. The `-p 8080:80` option connects port 8080 of the host machine to port 80 inside the container. This allowed me to access the Nginx web server through `localhost:8080` even though Nginx was running inside a container.

Another thing I learned was how the container lifecycle works. After stopping the Nginx container, I was able to see its stopped status before removing it. When `docker rm` is used, the container and data stored only inside its writable container layer are removed. This showed me why important application data should not depend only on a temporary container.

Containerization can also improve the way developers and IT operations teams work together. Developers can package applications with their needed components, while operations teams can deploy the same container more consistently in different environments. This can make deployment easier and reduce differences between development and production environments.

My GitHub portfolio is also becoming more organized as I complete each laboratory activity. It now contains documentation of my cloud computing activities, commands, screenshots, and reflections. This activity added my first hands-on experience with Docker and containerized web deployment to my portfolio.
