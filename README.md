# My Common Geodjango configs
A simple writeup of my common settings/configurations in jump-starting and deploying a geodjango application.

The procedures assume a linux OS, in my case Ubuntu 16.10. This should work fine with Ubuntu >=16.04.

## Install Python, Pip
 $ sudo apt-get install python-setuptools python-pip

## Create and setup vitrtualenv and virtualenvwrapper
  ### Install virtualenv using the pip installer:
    $ pip install virtualenv
 
 
## Install Django

## Install PostgresQL, Postgis, pgadmin3
 $ sudo apt-get update
 $ sudo apt-get install -y postgresql postgresql-contrib

## Install postgis
  $ sudo apt-get install -y postgis postgresql-9.5-postgis-2.2

## Install pgadmin3
 $ sudo apt-get install pgadmin3

## Install Geospatial Libraries
 $ sudo apt-get install binutils libproj-dev gdal-bin

## Change postgresql default password
 $ sudo su postgres
 $ psql
 ALTER USER Postgres WITH PASSWORD '';
