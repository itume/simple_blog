# simple_blog

First, run

    docker-compose build

Everytime you edit Gemfile, you run 'docker-compose build' and install gems

After that, you shoud edit password and host in config/databsase.yml
* host is mysql container name in docker-compose.yml(ex: db)
* password is in docker-compose.yml

Then, run this command for create database

    docker-compose run web rails db:create

Start

    docker-compose up

Open http://localhost:3000/


## operation

Stop

    docker-compose down

attach container

    docker exec -it #{container_name} bash

## Rails

rails new . -BCJS --skip-turbolinks --skip-webpack-install -d=mysql
