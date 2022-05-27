# Boilerplate for building Django Containers 

Standard starter template for django.

## Build Docker Image 

`docker build -t <name> .` 

This will build your container from the `dockerfile`. Feel free to change the dockerfile to fit your use case.

## Run the container interactively

```
docker run -it -p 8020:8020 \ 
  -e DJANGO_SUPERUSER_USERNAME=admin \ 
  -e DJANGO_SUPERUSER_PASSWORD=sekret1 \ 
  -e DJANGO_SUPERUSER_EMAIL=admin@example.com \ 
  [image_name]
```
