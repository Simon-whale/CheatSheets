# Docker 

## Docker Containers

This section will list all the commands that I know how to run on a container, some of these commands you can combine look at **List ids of all containers** and **Remove a container** can be combind to remove all containers that are in the Deamon.


**List all containers**
```
docker container ls -a
```

**List ids of all containers**
```
docker container ls -aq
```

**Remove a container**

Begin by getting the Id of the container, where xxx is the first 3 characters from the docker container Id
```
docker container rm xxx
```

**Remove all containers**

Please note that you will need to stop the containers before removing them
```
docker container rm (docker container ls -aq)
```

**Stopping a running container**

This example is done by passing the first 3 characters minimum from the of the container
```
docker container stop xxx
```

or 

the container name is the tag used to identified from list the containers, i.e. docker container ls -a
```
docker container stop container_name
```

## Docker Images

**List all images**
```
docker images ls
```

**List all Ids of images**
``` 
docker images -q
```

## Docker container logs

activity logs from a container 

``` 
docker container logs azurite
```

