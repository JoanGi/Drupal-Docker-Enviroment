# Drupal-Docker-Enviroment
<<<<<<< Updated upstream
A Docker Drupal LAMP Environment with HTTPS enabled with Let's Ecrypt ready to integration or test enviroment
=======

A Docker Drupal LAMP Environment with HTTPS enabled with Let's Ecrypt ready to integration or test enviroment.

Useful to integrate your Drupal APP with third-party consumers like mobile APP.

## Requeriments

- Docker
- Docker-compose
- Ubuntu Server
- You need to have a domain working (Traefik works with domains).

## Instructions

Set the variables with correct data in .env.
Set your Drupal code inside site/ folder.

Once this is done:

Go to the root (the folder where docker-compose.yml is:

$ docker-compose up -d

-d (to roll the processs in background).

Access to the container:

docker exec -it "YouProjectName_php" bash


## Tips


Data inside site/ and the data of the Databse will be persistant.

You .ssh keys are copied inside your Docker container, you can access your repositories without problem.

In docker-compose.yml uncomment Solr to have a ready-to-use Solr server (please use Drupal Search API to connect it).

In docker-compose.yml uncomment Node to have a node ready container node. Please set you node app inside /node folder before.

In docker-compose.yml in traefik label, you can set your own entry ports.



Base project from wodby  https://github.com/wodby/docker4drupal
>>>>>>> Stashed changes
