## Basic commands

### Pulling images

```
docker pull postgres:9.6
```

### Check images

```
docker images
```

### Run

Docker run runs a new container using an image
Docker start runs an existing container

```
docker run postgres:9.6
```

detached mode

```
docker run -d postgres:9.6
```

adding name

```
docker run -d postgres:9.6 --name my-redis-container
```

### Check running containers

```
docker ps
```

Check running/stop containers

```
docker ps -a
```

### Stop running containers

```
docker stop CONTAINER_ID
```

### Restart container

```
docker start CONTAINER_ID
```

### Binding to two different ports

```
docker run -{HOST_PORT}:{CONTAINER_PORT} redis
ex: docker run -p6000:6379 redis
```

### Checking logs

```
docker logs CONTAINER_NAME or CONTAINER_ID
ex: docker logs my-redis-container
```

### Login into container

```
docker exec -it CONTAINER_ID /bin/bash
ex: docker exec -it xxxxx /bin/bash
```
