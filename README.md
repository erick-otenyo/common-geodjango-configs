# My Common Geodjango configs
A simple writeup of my codmmon settings/configurations in jump-starting and deploying a geodjango application.

The procedures assume a linux OS, in my case Ubuntu 16.10. This should work fine with Ubuntu >=16.04.

## Install Python, Pip

## Create and setup vitrtualenv and virtuallenvwrapper

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
