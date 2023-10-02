# Docker Hub

Docker Hub is a public registry for Docker images. It provides a central place to store, share, and discover Docker images.

Docker Hub is a free service, but it also offers paid plans with additional features, such as private image repositories and automated builds.

To use Docker Hub, you need to create an account. Once you have created an account, you can start pushing and pulling Docker images.

To push a Docker image to Docker Hub, you can use the docker push command. To pull a Docker image from Docker Hub, you can use the docker pull command.

## Docker parent image

A Docker parent image is a Docker image that is used as the base for another Docker image. Parent images are typically used to provide common components, such as operating systems and runtimes, to other images.

When you create a Docker image, you can specify a parent image using the FROM directive in the Dockerfile. The parent image will then be used as the base for your image.

For example, if you want to create a Docker image for a Python web application, you could use the python:3.10 image as the parent image. This would provide your image with all of the necessary components to run a Python web application, such as the Python interpreter and standard library.

### Using parent images and Docker Hub

Using parent images and Docker Hub can help you to create and deploy Docker images more efficiently.

By using parent images, you can avoid duplicating the work of other Docker users. For example, if you need to create a Docker image for a Python web application, you can use the python:3.10 image as the parent image. This will save you from having to install Python and all of the necessary libraries in your own image.

Docker Hub makes it easy to share and discover Docker images. If you need to deploy your Docker image to a production environment, you can push your image to Docker Hub. You can then pull the image from Docker Hub to the production environment.
