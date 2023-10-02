# What is Docker

Docker is an open-source platform for developing, shipping, and running applications. It enables you to package your applications into containers, which are lightweight, standalone, executable packages of software that include everything needed to run an application: code, runtime, system tools, system libraries and settings.

### How Docker works

Docker works by creating lightweight, isolated environments called containers. Containers are created from Docker images, which are immutable templates that contain all the necessary files and dependencies to run an application.

It uses a client-server architecture with three key components:

- Docker Client: This is the command-line tool or API that allows users to interact with Docker.

- Docker Daemon: The Docker daemon is a background service responsible for building, running, and managing containers. It listens for Docker API requests and manages container lifecycle.

- Docker Registry: Docker containers can be stored in registries like Docker Hub or private registries. These registries serve as repositories for container images, which are used to create containers.

To create a container, you first need to create a Dockerfile. A Dockerfile is a text file that contains instructions for building a Docker image. Once you have created a Dockerfile, you can build a Docker image using the `docker build command`.

Once you have built a Docker image, you can run it using the `docker run command`. When you run a Docker image, Docker creates a container from the image. The container is isolated from other containers and the host operating system, and it has its own dedicated resources.

### Why use Docker?

- Consistency: Docker containers provide a consistent environment for running applications, regardless of the underlying infrastructure. This makes it easier to develop, test, and deploy applications.

- Portability: Docker containers can be run on any machine that has the Docker engine installed, making them easy to transport between different environments.

- Resource Efficiency: Docker containers share the underlying operating system kernel, which makes them more resource-efficient than virtual machines.

- Scalability: Docker containers can be easily scaled up or down to meet demand.

- Reproducibility: Docker images are immutable, which means that they can be reproduced exactly the same way each time. This makes it easier to ensure that applications are always running in a consistent environment.

- Collaboration: Docker containers make it easy to share applications with other developers and teams. This can help to improve collaboration and streamline the development process.

- Version Control: Docker can track versions of container image, allowing you to roll back to previous version, and trace who built a version and how.

## Docker Terms and Tools

- Docker images
- Docker containers
- DockerFile
- Docker Hub
