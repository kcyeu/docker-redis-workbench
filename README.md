# docker-redis-workbench

Dockerized Redis Workbench.

## Usage

To run the container, (optionally) start redis:

```
sudo docker run --name redis-server -d redis
```

, then do the following to start container with linked redis-server:

```
sudo docker run -d -p 80:80 --name redis-workbench --link redis-server:redis redis-workbench
```

