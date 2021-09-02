# Wordpress + Docker

## Description
Start developing a fresh php application with `docker` using `docker-compose`.

The images used in this repo is `wordpress 5.8` and `mysql:5.7`.
The goal is to make setting up the development as simple as possible.

wordpress latest version can install from here.
(this project wordpress version is 5.8)
```
https://wordpress.org/download/
```

## 1. Setup development environment
<!-- /TOC -->
### Prerequisites
In order to use this compose file (docker-compose.yml) you must have:

1. [docker](https://docs.docker.com/engine/installation/)
1. [docker-compose](https://docs.docker.com/compose/install/)

## 2. Start Up
* Go to Project Directory
```
cd [proj-path]

docker-compose up -d
```

* Reset docker-compose
```
docker-compose restart
```

## 3. Project Setting

### Change wordpress for local db at wp-config.php
```
db_name : wordpress
username : wordpress
password : wordpress
host : db:3306
```

### Run wordpress
* for wp-admin
```
http://localhost:3030/wp-admin/
```
* for phpmyamin
```
http://localhost:3333
username: wordpress
password: wordpress
```