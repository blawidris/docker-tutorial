# What is Docker

Docker is a containerization platform that allows developers to package an application and its dependencies into a self-contained unit called a container. This container can be easily deployed on any system that has Docker installed, without having to worry about the underlying system's configuration, libraries, or dependencies.

Docker uses a technology called containerization to achieve this level of portability and consistency across different environments. A container is a lightweight, standalone executable package that includes everything needed to run an application, including the code, runtime, system tools, libraries, and settings. Containers can be easily moved between different environments, from development to testing to production, without any changes to the code.

The benefits of using Docker include:

Consistency: Docker ensures that the same environment is used across all stages of the application lifecycle, from development to production.

Portability: Docker containers can be easily moved between different environments and platforms, without any changes to the application code.

Efficiency: Docker allows multiple containers to run on the same host, maximizing resource utilization and reducing costs.

Scalability: Docker makes it easy to scale an application horizontally by adding more containers.

Security: Docker provides a secure runtime environment for applications, with isolated containers and fine-grained control over access and permissions.

### Why do we use **Docker**

### Is it necessary to have Docker installed on the hosting server in order to deploy an application that was developed and packaged using Docker on a local machine?

If you have used Docker to package and deploy your application on your local machine, it is possible to deploy the same application on a live server without Docker. However, there are a few things to keep in mind.

First, you will need to ensure that the live server has all the dependencies and libraries required by your application. This may involve installing additional software or configuring the server environment to match your local development environment.

Second, you will need to ensure that your application is configured correctly for the live server environment. This may involve modifying configuration files, updating environment variables, or changing other settings that were specific to your local machine.

Finally, you will need to ensure that your application is deployed and configured correctly on the live server. This may involve setting up a web server, configuring DNS settings, and other tasks related to hosting and serving your application.

## Installation on Ubuntu

**Step 1:** update your pc packages index

```sudo apt-get update```

**Step 2:** Install Docker Engine, containerd, and Docker Compose.

``` sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin ```

**Step 3:** Verify that the Docker Engine installation is successful

```

// check composer version

docker compose version

// check docker version
docker --version

// running a hello-world image

sudo docker run hello-world

```

**Step 4:** Lauch Docker Desktop

```systemctl --user start docker-desktop
```

**Step 5:** Stop Docker Desktop

``` 
systemctl --user stop docker-desktop
```

#### To enable Docker Desktop to start on login

``` systemctl --user enable docker-desktop ```
