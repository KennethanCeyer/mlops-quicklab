<p align="center"><img width="150" src="../../assets/logo.png" alt="ops" /></p>
<h1 align="center">MLOps Quicklab</h1>
<p align="center">Docker Optimization</p>

## Installation

```bash
git clone https://github.com/KennethanCeyer/mlops-quicklab.git
cd dockers/optimization/
```

## Getting started

Build and push a base docker image.

> Change `{USERNAME}` to your [docker.io](https://docker.io/)'s username.

```bash
docker build . -t fastapi-app:base -f Dockerfile.base
docker tag fastapi-app:base {USERNAME}/fastapi-app:base

# Login to docker.io
docker login
docker push {USERNAME}/fastapi-app:base
```

Build a service docker image.

> Change `{USERNAME}` to your [docker.io](https://docker.io/)'s username.

```bash
docker build . -t fastapi-app:optmized
docker run \
    -dit -p 8000:8000 --name fastapi-app-test fastapi-app:optmized
curl http://localhost:8000
```
