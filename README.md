# My Common Geodjango configs
A simple writeup of my codmmon settings/configurations in jump-starting and deploying a geodjango application.

## Install Python, Pip

## Install Django

## Install PostgresQL, Postgis, pgadmin3
 sudo apt-get update
 sudo apt-get install -y postgresql postgresql-contrib

## Install postgis
  sudo apt-get install -y postgis postgresql-9.5-postgis-2.2

## install pgadmin3
 sudo apt-get install pgadmin3

## Install Geospatial Libraries
 sudo apt-get install binutils libproj-dev gdal-bin

## change postgresql default password
 sudo su postgres
 psql
 ALTER USER Postgres WITH PASSWORD '';
