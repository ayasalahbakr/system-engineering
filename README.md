# Assessment-App
By launching this application you will have an environment that contains mysql database attached to data container and nginx server on top of that there is a simple java springboot application that echo "Welcome To System Engineering Team" on the browser using nginx and the application connected to mysql database.

# Part 1: Docker

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for 

## Prerequisites
Docker-Composer needs to be installed on your local machine

## Installing
1) Browse to http://localhost:8123/
2) Error "This site can’t be reached" should be seen.
3) Run git clone https://github.com/ayasalahbakr/system-engineering.git
4) Run Jenkins Pipeline 
5) Browse again to http://localhost:8123/

You should see "Welcome To DevOps World"

## Built With
1) Java Springboot Platform for running the application
2) Docker-Composer to build the environment (application + MySql + Data Conatiner + Nginx)
3) Some shell commands to generate ssl self signed certificate and dhparam key
    * For generating ssl certificate:
        - openssl req -x509 -sha256 -nodes -newkey rsa:2048 -days 365 -keyout localhost.key -out    localhost.crt
    * For generating dhparam key:
        - openssl req -x509 -sha256 -nodes -newkey rsa:2048 -days 365 -keyout localhost.key -out localhost.crt
        - openssl dhparam -out dhparam.pem 1024
