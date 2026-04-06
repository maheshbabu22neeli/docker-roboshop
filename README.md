# docker-roboshop
Creating roboshop application using docker



- Disconnect the containers from existing default bridge network and connect to roboshop network
- ```shell
docker network create roboshop

docker network disconnect bridge mongodb
docker network disconnect bridge catalogue

docker network connect roboshop mongodb
docker network connect roboshop catalogue
```
- 