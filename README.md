<p align="center">
<a href="https://docs.djangoproject.com/" target="_blank">
<img src="logo.svg" width="400" alt="Logo">
</a></p>

___

## Install Poetry

```shell
curl -sSL https://install.python-poetry.org | python3 -
# of on MacOS
brew install poetry

poetry self update
```

## Install command reads the pyproject.toml file from the current project

```shell
# Set Up a Programming Environment
python3 -m venv venv
source venv/bin/activate

# Install Package
poetry install

# Show command to view all installed dependencies
poetry show --tree  --outdated

# Deactivate the environment
deactivate
```

### Run program

```shell
py app.py

```

```shell

pytest
pytest -v
coverage run -m pytest
coverage report
coverage html


```

# Documentation

### [Python Documentation](https://docs.python.org)

### [Apache Kafka](https://kafka.apache.org/quickstart)

```shell
start https://www.apache.org/dyn/closer.cgi?path=/kafka/3.4.0/kafka_2.13-3.4.0.tgz
```

# Docker

```shell
docker kill $(docker ps -aq); docker rm $(docker ps -aq); docker rmi $(docker images -aq); docker volume prune -f;

make stop-user-development; make build-user-development; make start-user-development
make stop-user-production; make build-user-production; make start-user-production
```

# [SQL Alchemy](https://www.sqlalchemy.org/)

## [SQL Alchemy Core](https://docs.sqlalchemy.org/en/20/core/index.html)

Database URLs

```shell
dialect+driver://username:password@host:port/database
```

The MySQL dialect uses mysqlclient as the default DBAPI. There are other MySQL DBAPIs available, including PyMySQL:

```shell
# default
engine = create_engine("mysql://scott:tiger@localhost/foo")

# mysqlclient (a maintained fork of MySQL-Python)
engine = create_engine("mysql+mysqldb://scott:tiger@localhost/foo")

# PyMySQL
engine = create_engine("mysql+pymysql://scott:tiger@localhost/foo")
```

## [Django Command Line Interface](https://docs.djangoproject.com/en)

```shell
python -m django --version
python manage.py runserver 0.0.0.0:8000
```