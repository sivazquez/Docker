# Docker
Docker files for different technologies

## Postgres
Docker FROM postgres:13.1
### Build
docker build -t {{IMAGE LABEL NAME}} .
### Run
docker run -d --name postgres-13-local \
-p {{PORT HOST}}:{{PORT DOCKER}} \
-e POSTGRES_PASSWORD={{PASSWORD}} \
-e POSTGRES_USER={{PASSWORD}} \
-e POSTGRES_DB={{DATABASE}} \
-v {{ROUTE HOST VOLUME}}:/var/lib/postgresql/data \
{{IMAGE LABEL NAME FROM BUILD}}

