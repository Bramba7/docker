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


#### Pull container

First step pull the bramba/awscli container to your docker environment.

```
docker pull bramba/awscli
```

#### Aws Configuration (linux and MacOs)
Use [nano](https://nano-editor.org/), or other txt editor to create the aws credential config file:
```
nano ~/.aws/credentials
```
Copy the example below, and replace information without the "<>". :

```
[default]
aws_access_key_id= <ACCESS KEY ID>
aws_secret_access_key= <SECRET KEY>
```

Next step is to create another file containing more information.
```
nano ~/.aws/config
```

In the settings below, the zone must be inserted, and also the type of output file that can be "JSON" or "YAML"
```
[default]
region=<Location>
output=<File type>
```
## Usage

#### Simple example

```shell
docker run -rm -it bramba/awscli --version
```

#### Checking S3 bucket list
```shell
docker run -it -v ~/.aws:/root/.aws bramba/awscli s3
```

