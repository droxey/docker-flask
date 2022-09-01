# docker-flask

<!-- omit in toc -->
## Table of Contents

1. [1. Build the Image](#build-the-image)
1. [2. Run the Container](#build-the-container)
1. [3. Access via Browser](#access-via-browsers)

## Command Reference

### 1. Build the Image

```bash
docker build -t flask-image .
```

### 2. Run the Container

```bash
docker run -p 5001:5000 --rm --name flask-container flask-image
```

### 3. Access via Browser

http://localhost:5001
