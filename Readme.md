# Docker Tutorial:

Is an isolated virtualized environment that allows developers to build, deploy and test applications.

It has some terminologies that one must understand in other to fully use the environment, which are:

1. Image: these are read-only layers that are immutable but contain the source code, tools, dependencies, libraries and other files needed for an application run. It represents templates i.e an application and its virtual environment at a specific point in time and cannot be run.
2. Container: it is used to create instances of an image which are mutable (writable). When a container is run, it adds a writable layer on top of the image's immutable layers, allowing you to run and modify software in an isolated environment.
   Docker container has the following features:
   Standardization ensures your application runs consistently across various environments, from development to production. This consistency is achieved because containers encapsulate the application's runtime environment, including libraries, configurations, and more, in a standardized format.
   Portable: It allows container images to be run on various hosts without the need to modify the application or its dependencies, enabling consistent behavior across different environments.
   Lightweight: It allows container images to utilize one machine, share its kernel, and virtualize the operating system to run isolated processes unlike virtual machines (VMs) where virtualization happens at the hardware level, containers virtualize at the app layer.
   Security: Container provides strong isolation, ensuring all running containers do not interrupt one another and making sure they are supported by the server.
   Isolation: It is the practice of separating and protecting different applications and processes from one another i.e. ensuring that each container operates in its own isolated environment which prevents conflicts between applications, ensures security by containing breaches, and enhances overall stability.

### Dockerfile

This is text files that contain the instruction to build a docker image. It defines the environment, configurations, dependencies, and other settings required to create a consistent and reproducible image for running applications in Docker containers.
_DockerFile Principle_
It’s case-insensitive but it convention is to use uppercase
Must begin with FROM
Use # as a comment

### Why do we use Dockerfile

Ensures docker images can be reproduced no matter where dey are built or deployed
It allows you to track changes to the image-building process over time, aiding collaboration and troubleshooting (version control)
It promotes uniformity whereby everyone in the team can use the same Dockerfile
It automates the process of building a Docker image
It allows you to control what software is installed in your image, reducing the attack surface by excluding unnecessary packages.

### Parser Directive

It is a special comment that provides instructions to the Docker build process about how to interpret certain lines in the Dockerfile. It helps control the behavior of Docker's parser when reading and executing the Dockerfile instructions. It must be written as a comment at the beginning line and it starts with a special syntax: # syntax=<parser_name>[parser_option]. Here, parser_name is the name of the parser, and parser_option is an optional parameter.

e.g


```
# syntax=docker/dockerfile:1.2
FROM ubuntu:latest
```
