# Docker 
## Introduction to Container
Virutal Mechine (VM)
## Introduction to Docker
Docker is container manager. It is free and Open Source application and it is released in 2013. 
## How to install Docker
## Docker Architecture

## Docker Image
`docker image ls` to show list image.

`docker pull nameimage:tag` to download docker image. Default tag will set in latest. Once yo have downloaded image, docker will not download again.

`docekr image rm nameimage:latest` to remove docker image
## Docker Registry
Docker is place to store docker image. Docker image that have stored in docker registry, can be used by docker demon.

Kind of docker registry:
1. Docker Hub : https://hub.docker.com/
2. Digital Ocean Container Registry : https://www.digitalocean.com/products/container-registry/
3. Google Cloud Container Registry : https://cloud.google.com/container-registry
4. Amazon Elastic Container Registry : https://aws.amazon.com/id/ecr/
5. Azure Container Registry : https://azure.microsoft.com/en-us/services/container-registry/

## Docker Container
One docker image can be used to create some container on condition that you create different name of container. Once you have installed container, the image cannot be removed. When you want to remove the image, you have to remove the container first. 

Status container in default is not running. When you want to run containe, you have to start the container. To get list of container in Docker Daemond you can commit this task `docker container ls -a`. You can also show only list container is running run this command `docker container ls`.

To create container you can run `docker container create --name namecontainer image:redis`. When it is created you can get the container ID. When you create container while the image is not available. Docker will download the image automatically.

Next, we can run the container in this command `docker container start containerID/namecontainer`. When you run `docker container ls`, it show the **contohregis** container is running. Run `docker container stop contohredis` to stop container and status contohredis in `docker container ls -a` will set ***Exited**. You can see log the container run this command `docker container logs -f connectorid/namecontainer`

When you want to remove container, you can run `docker container rm namecontainer` then check list of container `docker container ls -a` to ensure that the container is remove.

## Docker Volume
## Docker Network


