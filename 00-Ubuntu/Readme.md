**Start Bash inside Ubuntu**:

```shell script
docker run -it ubuntu:18.04
```

or 

```shell script
docker run --name ubuntu-playground --rm -it ubuntu:18.04
```

**List running containers**:

```shell script
docker ps
```

**List all containers (stopped ones as well)**:

```shell script
docker ps -a
```

**Get diff of playground container**:

```shell script
docker diff ubuntu-playground
```