# Docker inside Docker
### version 1.2.8
![Docker Image Version (latest by date)](https://img.shields.io/docker/v/bramba/dockerdocker?color=green&logo=docker)
![Docker Pulls](https://img.shields.io/docker/pulls/bramba/dockerdocker?color=green&logo=docker)
![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/bramba/dockerdocker?color=green&logo=docker)

A one paragraph description about the container.

## Getting Started

These instructions will cover usage information and for the docker container 

### Prerequisites


In order to run this container you'll need docker installed.

* [Windows](https://docs.docker.com/windows/started)
* [OS X](https://docs.docker.com/mac/started/)
* [Linux](https://docs.docker.com/linux/started/)

### Usage

#### Pull :

```shell
docker pull bramba/dockerdocker
```

#### Example to check if the container is working:

```shell
docker run --rm -v "/var/run/docker.sock:/var/run/docker.sock" bramba/dockerdocker /bin/sh -c "docker ps"
```
#### Example of access to container shell:

```shell
docker run -it -v "/var/run/docker.sock:/var/run/docker.sock" bramba/dockerdocker /bin/sh
```
