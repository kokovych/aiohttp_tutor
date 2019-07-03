## Simple aiohttp-based project

This project is created with education purpose: get practice experience
with aiohttp.

Used python 3.5+ (3.6.8), postgres 11. 

#### Preparation

1. Create and activate virtual environment:

```sh 
$ virualenv -p python3 venv
$ source venv/bin/activate
```

2. Install requirements:
```
(venv)$ pip install  -r requirements.text
```

3. Create database and database user:

```
$ psql -U postgres -h localhost
> CREATE DATABASE aiohttpdemo_polls;
> CREATE USER aiohttpdemo_user WITH PASSWORD 'aiohttpdemo_pass';
> GRANT ALL PRIVILEGES ON DATABASE aiohttpdemo_polls TO aiohttpdemo_user;

```

#### Run

For start project:

```
(venv)$ python aiohttpdemo_polls/main.py
```