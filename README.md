# Nginx-Performance-Workshop
Setup Nginx for hight perfomance requirements.
Gain insights into optimization strategies for a nginx deployments and scale to around 1k-10k+ request concurrently with just a single instance (see the notes at the specific configurations).

## Learned
- basic usage of nginx

## Prerequisites
Since this project was build with docker there is a small amount of prerequisites
- docker
- access to docker-hub

## Getting Started
### Run image from docker-hub
- run container
```
docker run --name my-nginx -p 3000:80 -d <docker-registry-user>/nginx-static-site-test:latest
```
- access localhost:3000

### Build and run own image
- build image
```
docker build -t custom-nginx .
```
- run image
```
docker run --rm -p 3000:80 --name my-nginx my-nginx
```
- access localhost:3000


## Important commands
- tag image (example)
```
docker tag c056598acb45 <docker-registry-user>/nginx-static-site-test
```
- push image to docker-hub (example)
```
docker push <docker-registry-user>/nginx-static-site-test
```

## Build with
- nginx
- docker
