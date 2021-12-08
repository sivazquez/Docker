# Docker
Docker files for different technologies

## Postgres
Docker FROM postgres:13.1
### Build
docker build -t {{IMAGE LABEL NAME}} .
### Run
docker run -d --name {{NAME OF CONTAINER}} \
-p {{PORT HOST}}:5432 \
-e POSTGRES_PASSWORD={{PASSWORD}} \
-e POSTGRES_USER={{PASSWORD}} \
-e POSTGRES_DB={{DATABASE}} \
-v {{ROUTE HOST VOLUME}}:/var/lib/postgresql/data \
{{IMAGE LABEL NAME FROM BUILD}}

## LUMEN FRAMEWORK
Docker FROM lumen - framework for laravel
### Build
docker build -t {{IMAGE LABEL NAME}} .
### Run
docker run -d \
--name {{NAME OF CONTAINER}} \
-p {{PORT HOST}}:80 \
-v {{ROUTE HOST VOLUME}:/var/www/html  \
{{IMAGE LABEL NAME FROM BUILD}}

## Angular
inside the angular project add the dockerfile and docker-compose.yml files
### Build and Run
docker-compose up -d
