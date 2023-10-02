# Docker Containers

A Docker container is a running instance of a Docker image. Containers are isolated from each other and the host operating system, and they have their own dedicated resources.

Docker containers were once known as isolated processes. They run instances of Docker images, and they are virtualized runtime environments where applications are isolated from the underlying system.

Docker containers have their own file systems, networking, and storage. They depend on Docker images, and they use images to construct a runtime environment and run applications.

Unlike virtual machines, where virtualization occurs on the hardware level, Docker containers virtualize at the app layer. This means that Docker containers are more lightweight and portable than virtual machines.

![Containers](https://phoenixnap.com/kb/wp-content/uploads/2021/04/container-vs-virtual-machine.png)

### Docker container features

- **Standardization**: Docker containers ensure that applications are working in identical circumstances. This makes it easy to share applications with other team members.

- **Security**: Docker containers provide strong isolation, ensuring that each container does not interrupt another while running. This helps to improve the security of applications.

- **Lightweight**: Docker containers utilize one machine, share its kernel, and virtualize the operating system to run isolated processes. This makes Docker containers more lightweight and resource-efficient than virtual machines.

- **Portability**: Docker containers can be run on any machine that has the Docker engine installed, making them easy to transport between different environments.

- **Scalability**: Docker containers can be easily scaled up or down to meet demand.

- **Reproducibility**: Docker containers are created from images, which are immutable. This makes it easy to reproduce Docker containers exactly the same way each time.

### Difference between Docker image and container

| Type       | Template                 | Running Instance of a Template              |
| ---------- | ------------------------ | ------------------------------------------- |
| Mutability | Immutable                | Mutable                                     |
| Scope      | Can be shared and reused | Isolated to the machine where it is running |
| Use case   | Used to build containers | Used to run applications                    |
