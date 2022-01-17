# little introduction

- Docker Compose is used to run multiple containers as a single service. For .
a tool for defining and running multi-container Docker applications
 
- With Compose, we can create a YAML file to define the services and with a single command, can spin everything up or tear it all down
MEANS you use a YAML file to configure your application’s services. Then, with a single command, you create and start all the services from your configuration

Example : suppose you had an application which required NGNIX and MySQL, you could create one file which would start both the containers as a service without the need to start each one separately

## three-step process:

    1. Define your app’s environment with a Dockerfile so it can be reproduced anywhere.

    2. Define the services that make up your app in docker-compose.yml so they can be run together in an isolated environment.

    3. Run docker compose up and the Docker compose command starts and runs your entire app. You can alternatively run docker-compose up using the docker-compose binary.

## Pros

a big advantage of using Compose is you can define your application stack in a file, keep it at the root of your project repo (it’s now version controlled), and easily enable someone else to contribute to your project. Someone would only need to clone your repo and start the compose app. In fact, you might see quite a few projects on GitHub/GitLab doing exactly this now

## Cons

you can't use docker compose in production, because it's not design for it 
u can't do rolling updates without downtime using compose, instead u have to bring all the containers down, change the images and finally bring up new containers    
wasn't designed for the production concepts like "always uptime" or "multiservers"
doesn't have a database working in background and storing information