# My Common Geodjango configs
A simple writeup of my common settings/configurations in jump-starting and deploying a geodjango application.

The procedures assume a linux OS, in my case Ubuntu 16.10. This should work fine with Ubuntu >=16.04.

## Install Python, Pip
 $ sudo apt-get install python-setuptools python-pip

## Create and setup virtualenv and virtualenvwrapper
  ### Install virtualenv using the pip installer:
      $ pip install virtualenv
 ### Install virtualenvwrapper using easy_install:
     $ sudo easy_install virtualenvwrapper
 ### Assign the WORKON_HOME variable to your home directory with the folder name venvs. Create a single folder where you want to store all your different Python virtual environments; in my case, the folder is located at /home/oty/venvs :
     $ export WORKON_HOME=~/venvs
     $ mkdir $WORKON_HOME
 ### Run the source command to execute the virtualenvrapper.sh bash file:
     $ source /usr/local/bin/virtualenvwrapper.sh
 ### Next, we create a new virtual environment called pygeoan_cb , and this is also the name of the new folder where the virtual environment is installed:
     $ mkvirtualenv env
   To use virtualenvwrapper the next time you start up your machine, we need to
set it up so that your bash terminal runs the virtualenvwrapper.sh script when
your computer starts

 ### First, put it in your ~/.bashrc file:
     $ echo "export WORKON_HOME=$WORKON_HOME" >> ~/.bashrc
 ### Next, we'll import the virtualenvwrapper function in our bash:
     $ echo "source /usr/local/bin/virtualenvwrapper.sh" >> ~/.bashrc
 ### Now we can execute our bash:
     $ source ~/.bashrc
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
