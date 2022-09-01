# docker-flask

<!-- omit in toc -->
## Table of Contents

1. [Command Reference](#command-reference)
   1. [Build the Image](#build-the-image)
   1. [Run the Container](#build-the-container)
   1. [Access via Browser](#access-via-browsers)

## Command Reference

### Build the Image

```bash
docker build -t flask-image .
```

### Run the Container

```bash
docker run -p 5001:5000 --rm --name flask-container flask-image
```

### Access via Browser

http://localhost:5001
