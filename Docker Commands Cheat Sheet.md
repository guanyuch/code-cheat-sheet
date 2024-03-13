# **Docker Commands Cheat Sheet**

## **Basic Commands**

#### List Docker CLI commands
- `docker`

#### Display Docker version and info
- `docker --version`
- `docker version`
- `docker info`

#### Execute Docker image
- `docker run IMAGE_NAME`

#### List running containers
- `docker ps`

#### List all containers (running and stopped)
- `docker ps -a`

#### Stop a running container
- `docker stop CONTAINER_ID`

#### Start a stopped container
- `docker start CONTAINER_ID`

#### Remove a stopped container
- `docker rm CONTAINER_ID`

#### Pull an image from a Docker registry
- `docker pull IMAGE_NAME`

#### Build an image from a Dockerfile
- `docker build -t IMAGE_NAME:TAG .`

#### List Docker images
- `docker images`

#### Remove Docker image
- `docker rmi IMAGE_ID`

## **Docker Compose Commands**

#### Build services defined in docker-compose.yml
- `docker-compose build`

#### Start services defined in docker-compose.yml
- `docker-compose up`

#### Stop services started with docker-compose up
- `docker-compose down`

#### List the status of running services
- `docker-compose ps`

## **Docker Volume Commands**

#### Create a volume
- `docker volume create VOLUME_NAME`

#### List volumes
- `docker volume ls`

#### Remove a volume
- `docker volume rm VOLUME_NAME`

#### Inspect a volume
- `docker volume inspect VOLUME_NAME`

## **Docker Network Commands**

#### List networks
- `docker network ls`

#### Create a network
- `docker network create NETWORK_NAME`

#### Remove a network
- `docker network rm NETWORK_NAME`

#### Inspect a network
- `docker network inspect NETWORK_NAME`

## **Docker Image and Container Management**

#### Tag a local image with a new name
- `docker tag SOURCE_IMAGE[:TAG] TARGET_IMAGE[:TAG]`

#### Push an image to a registry
- `docker push IMAGE_NAME:TAG`

#### Save an image to a tar archive
- `docker save -o FILENAME.tar IMAGE_NAME:TAG`

#### Load an image from a tar archive
- `docker load -i FILENAME.tar`
