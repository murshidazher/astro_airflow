# astro_airflow
An example astro airflow playground

## Astronomer CLI

### Install astro cli

- [astronomer install cli docs](https://www.astronomer.io/docs/astro/cli/install-cli)

### Creating a new project

> [astronomer docs](https://www.astronomer.io/docs/astro/cli/astro-dev-init/)

```sh
astro dev init
```

## Up & Running

> login credentials - admin:admin

```sh
astro dev start

# to install requirements 
astro dev restart
```

```sh
astro dev stop
```

## Spark setup

```sh
cd spark/master
docker build -t airflow/spark-master .

cd spark/worker
docker build -t airflow/spark-worker .

cd spark/notebooks/stock_transform
docker build -t airflow/stock-app .
```