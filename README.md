# docker-roboshop
Creating roboshop application using docker



- Disconnect the containers from existing default bridge network and connect to roboshop network
```shell
docker network create roboshop

docker network disconnect bridge mongodb
docker network disconnect bridge catalogue

docker network connect roboshop mongodb
docker network connect roboshop catalogue
```


##  Docker Compose
- it is an YAML file which defines the services, networks and volumes for our application.
- It can build the images.
- It can define the dependencies between the containers/components.
- It can start all the containers at a a time based on dependency.
- It can stop all the containers at a time based on dependency.

```shell
docker compose build

docker compose up -d

docker compose up -d --build (to rebuild the application)
```