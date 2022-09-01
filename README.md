# docker-flask

<!-- omit in toc -->
## Table of Contents

1. [Command Reference](#command-reference)
   1. [Build the image](#build-the-image)
   1. [Build the container](#build-the-container)
   1. [Remove all images with names that contain `flask`](#remove-all-images-with-names-that-contain-flask)
   1. [Remove all containers with names that contain `flask`](#remove-all-containers-with-names-that-contain-flask)
   1. [See what's running](#see-whats-running)

## Command Reference

### Build the image

```bash
docker build -t flask-image .
```

### Run the container

```bash
docker run -p 5001:5000 --rm --name flask-container flask-image
```

### Remove all images with names that contain `flask`

```bash
docker images -a | grep "flask" | awk '{print $3}' | xargs docker rmi
```

### Remove all containers with names that contain `flask`

```bash
docker ps -a | grep "flask" | awk '{print $3}' | xargs docker rmi
```

### See what's running

```bash
docker ps --format '{{.Names}}'
```
### Access via Browser

http://localhost:5001
