# Docker Aws-Cli
![Docker Image Version (latest by date)](https://img.shields.io/docker/v/bramba/awscli?color=green&logo=docker)
![Docker Pulls](https://img.shields.io/docker/pulls/bramba/awscli?color=green&logo=docker)
![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/bramba/awscli?color=gren&logo=docker)


  This container has the objective of simple access to Amazon console. In addition, 
the container was created on top of the Alpine operating system, where the purpose is to 
make the container as small as possible.

## Getting Started

These instructions will cover usage information and for the docker container 

### Prerequisities


In order to run this container you'll need docker installed.

* [Windows](https://docs.docker.com/windows/started)
* [OS X](https://docs.docker.com/mac/started/)
* [Linux](https://docs.docker.com/linux/started/)

### Usage

#### Pull container

```shell
docker pull bramba/awscli
```

#### Simple example

```shell
docker run -rm -it bramba/awscli --version
