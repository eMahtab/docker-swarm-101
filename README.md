## Docker Swarm & Stack Tutorial

Video Tutorial: https://youtu.be/m6WgX_LBtEk

To run this locally, run:

```
docker swarm init
git clone https://github.com/eMahtab/docker-swarm-101.git
cd docker-swarm-101
docker build -t hello:1.0 -f hello-service/Dockerfile hello-service
docker build -t goodbye:1.0 -f goodbye-service/Dockerfile goodbye-service
docker stack deploy -c ./docker-compose.yml talk
```

To tear down the stack:
```
docker stack rm talk
```
