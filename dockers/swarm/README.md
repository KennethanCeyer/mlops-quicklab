<p align="center"><img width="150" src="../../assets/logo.png" alt="ops" /></p>
<h1 align="center">MLOps Quicklab</h1>
<p align="center">Docker Swarm</p>

## Installation

```bash
git clone https://github.com/KennethanCeyer/mlops-quicklab.git
cd dockers/swarm/
```

## Swarm settings

You need setup docker swarm with multiple nodes.

> Check [this document](https://docs.docker.com/engine/swarm/swarm-tutorial/create-swarm/) to setup your swarm environment.

```bash
docker swarm init
```

## Getting started

```bash
docker stack deploy \
    --compose-file docker-compose.yml \
    fastapi
```

## Load Testing

```bash
pip3 install -r requirements.txt
locust -f locustfile.py
```
