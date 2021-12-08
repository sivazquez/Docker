FROM postgres:13.1

### ===================================================================== ###
### Instalando la extension postgis para trabajar con datos geoespaciales
### ===================================================================== ###
RUN apt-get update \
    && apt-get install wget -y \
    && apt-get install postgresql-13-postgis-3 -y \
    && apt-get install postgis -y

### ===================================================================== ###
### este .sql contiene la instruccion para crear la extension en la db
### ===================================================================== ###
COPY ./db.sql /docker-entrypoint-initdb.d/