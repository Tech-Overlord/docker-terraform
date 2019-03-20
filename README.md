[![license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://github.com/Tech-Overlord/dockerterraform/blob/master/LICENSE) 

# docker-terraform
Docker containers that have Terraform pre-installed and available to be used right away.

* Terraform version currently available in Docker Images: `0.11.13`

# Supported tags and Dockerfile:

For Ubuntu 18.04 (bionic), docker tag and Docker file:
* [ubuntu1804](https://github.com/Tech-Overlord/docker-terraform/blob/master/ubuntu/bionic/Dockerfile)

For Ubuntu 16.04 (xenial), docker tag and Docker file:
* [ubuntu1604](https://github.com/Tech-Overlord/docker-terraform/blob/master/ubuntu/xenial/Dockerfile)

For CentOS7, docker tag and Docker file:
* [centos7](https://github.com/Tech-Overlord/docker-terraform/blob/master/centos/7/Dockerfile)

# How to use:
Simply pull the docker image using whichever tag you prefer or run it directly.

For instance, if you would like to use a Ubuntu 18.04 (bionic) container with pre-installed Terraform, then run the following and you will have interactive access to the container:

```shell
docker run -it darkwizard242/terraform:ubuntu1804 /bin/bash 
```

This will pull the image down and then attach to the container.


Similarly, for using Terraform in a Ubuntu 16.04 (xenial) container or a CentOS7 container.
```shell
docker run -it darkwizard242/terraform:ubuntu1604 /bin/bash
```
or
```shell
docker run -it darkwizard242/terraform:centos7 /bin/bash
```


**Note:** Image tag `latest` (i.e. darkwizard242/terraform:latest ) has Ubuntu1804 as the underlying container image.