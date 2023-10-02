# Docker images

A Docker image is a read-only template that contains all the necessary files and dependencies to run an application. Docker images are sometimes referred to as snapshots due to their read-only quality.

Docker images are created using Dockerfiles, which are text files that contain instructions for building an image. Docker images can be created from one or more base images, which are pre-built images that contain common components, such as operating systems and runtimes.

Docker images are immutable, which means that once they are created, they cannot be changed. This makes it easy to ensure that applications are always running in a consistent environment.

Docker images consist of a series of layers. When a container is started up, a virtual environment is created from the image's layers. This allows developers to test and experiment with software in a stable and uniform condition.

Docker images have multiple layers, each one originates from the previous layer but is different from it. 

![Images](https://phoenixnap.com/kb/wp-content/uploads/2021/04/container-layers.png)

### Anatomy of a Docker image

The anatomy of a Docker image can be divided into the following parts:

* **Base layer**: The base layer is the bottom layer in a Docker image. It typically contains a minimal operating system and runtime environment.
* **Intermediate** layers: Intermediate layers are added to the base layer to add additional dependencies, such as libraries, tools, and application code.
* **Top layer**: The top layer in a Docker image is the application layer. It contains the application code and any configuration files that are needed to run the application.

When a Docker image is built, the base layer is created first. Then, each intermediate layer is added to the base layer, one by one. Finally, the application layer is added to the top of the stack.

When a Docker container is created from a Docker image, the Docker engine starts by creating a writable layer on top of the image's layers. This writable layer is where the container's changes to the filesystem will be stored.

The Docker engine then mounts the image's layers on top of the writable layer. This allows the container to access the files and dependencies that it needs to run.

Docker images are immutable, which means that they cannot be changed once they are created. This makes Docker images very efficient, as the Docker engine can simply reuse the existing image layers when it creates new containers.
