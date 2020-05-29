# Wordpress Container 

## Docker Images

- https://hub.docker.com/_/wordpress/
- https://hub.docker.com/_/mariadb

## Run Containers

#### Config File "env-template"

```bash
MYSQL_USER=db-user
MYSQL_PASSWORD=db-password
MYSQL_DATABASE=db-name

WORDPRESS_DB_USER=db-user
WORDPRESS_DB_PASSWORD=db-passwrod
WORDPRESS_DB_NAME=db-name
```

#### Rename File "env-template"

```bash
mv env-template .env
```

#### Run Project

```bash
## Run container
docker-compose up
## or background
docker-compose up -d 
## or background and build
docker-compose up -d --build
```