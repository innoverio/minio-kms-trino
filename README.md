# Zero Trust Data Access using minio and Trino

In this tutorial you will setup trino, minio, kes and communicate with an external KMS system (AWS Secrets Manager/KMS in this case).

Follow along with [the tutorial](https://medium.com/@mdesmet_7096/zero-trust-data-access-using-minio-and-trino-6140f78f410f)

## Prerequisites

In order to use this repository you need to have [Docker](https://www.docker.com/why-docker) installed to run your service [containers](https://www.docker.com/why-docker). Check if you have Docker installed by running `docker --version`. If Docker isn't found, please refer to the [install insructions](https://docs.docker.com/engine/install/) and install Docker before trying to run these tutorials. If you're on mac or windows, you will just need to install docker desktop. If you're on a linux distribution, you will just need to install the docker engine.

## Helpful Docker commands

### Start Service

`docker-compose up -d`

### Stop Service

`docker-compose stop`

### Clean Service

[cleans images, containers, and network](shttps://docs.docker.com/config/pruning/)

`docker system prune --all --force`

[cleans volumes](shttps://docs.docker.com/config/pruning/)

`docker volume prune --force`

### Show Service Images 

`docker images`

### Login to Container

`docker container exec -it <container_id> /bin/bash`

### Show Service Logs

`docker logs <container_id>`

### List Services

`docker container ls`

### List Service Process information

`docker-compose ps`