# Boilerplate for building Django Containers 

[![Docker Image CI](https://github.com/jharleydev/django-container-template/actions/workflows/docker-build-push.yml/badge.svg?branch=main)](https://github.com/jharleydev/django-container-template/actions/workflows/docker-build-push.yml)   [![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](gitpod#https://github.com/jharleydev/django-container-template)


Standard starter template for django.

## Build Docker Image 

`docker build -t <name> .` 

This will build your container from the `Dockerfile`. Feel free to change the dockerfile to fit your use case.

## Run the container interactively

```
docker run -it -p 8020:8020 \ 
  -e DJANGO_SUPERUSER_USERNAME=admin \ 
  -e DJANGO_SUPERUSER_PASSWORD=sekret1 \ 
  -e DJANGO_SUPERUSER_EMAIL=admin@example.com \ 
  [image_name]
```
