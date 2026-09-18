# Mission Reflection

This laboratory activity helped me understand the difference between using a Virtual Machine and using a Docker container. When setting up a Virtual Machine, an entire operating system has to be installed and started before the application can be used. This can take several minutes and requires more memory and storage. With Docker, the Nginx container was ready to run after pulling the image, and there was no need to install another operating system. This made the setup process much faster and showed me why containers are useful for deploying applications.

The port mapping `-p 8080:80` is necessary because the Nginx web server is running inside the container on port 80. Port 8080 on the host machine is connected to that port, allowing me to access the web server using `http://localhost:8080`. Without the port mapping, the service running inside the container would not be directly accessible through that host port.

When `docker rm` is used, the container itself is removed from Docker. Any data stored only inside the container can also be lost after the container is removed. This is why important data should be stored using Docker volumes or another persistent storage method instead of relying only on the container's filesystem.

Containerization also changes how developers and IT operations teams work together. Developers can package an application and its required environment into an image, while operations teams can use the same image when deploying the application. This can reduce differences between development and deployment environments and make the deployment process easier to repeat.

My GitHub portfolio is also becoming more organized as I add each laboratory activity. This activity added practical Docker experience to my previous cloud computing work. The screenshots and Markdown documentation also give me a record of the commands I used and what I learned from the activity.
