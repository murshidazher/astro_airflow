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
```