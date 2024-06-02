<p align="center"><img width="150" src="../assets/logo.png" alt="ops" /></p>
<h1 align="center">MLOps Quicklab</h1>
<p align="center">Airflow Basic</p>

## Installation

```bash
git clone https://github.com/KennethanCeyer/mlops-quicklab.git
cd airflow/basic/
```

## File structure

```plaintext
airflow/basic/
├── README.md
├── dags
│   ├── bigquery_airflow_example.py
│   └── bigquery_to_huggingface.py
├── docker-compose.yaml
├── logs
└── plugins
```

## Getting started

```bash
echo -e "AIRFLOW_UID=$(id -u)" > .env
```

## Run

```bash
docker compose up -d
```

## Cleanup

```bash
docker compose down --volume --rmi all
```
