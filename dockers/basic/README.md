<p align="center"><img width="150" src="../../assets/logo.png" alt="ops" /></p>
<h1 align="center">MLOps Quicklab</h1>
<p align="center">Docker Basic</p>

## Installation

```bash
git clone https://github.com/KennethanCeyer/mlops-quicklab.git
cd dockers/basic/
```

## Getting started

```bash
docker build . -t fastapi-app:latest
docker run \
    -dit -p 8000:80 --name fastapi-app-test fastapi-app:latest
curl http://localhost:8000
```

## Analysis your docker image by [Dive](https://github.com/wagoodman/dive)

Install [Dive](https://github.com/wagoodman/dive) by following the instruction.

> Check [Dive Installation](https://github.com/wagoodman/dive#installation) document.

Show built image by using the following command.

```bash
dive fastapi-app:latest
```
