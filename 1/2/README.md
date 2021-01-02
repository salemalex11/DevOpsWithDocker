# 1.2 Cleanup

## Exercise

We’ve left containers and a image that won’t be used anymore and are taking space, as `docker ps -as` and `docker images` will reveal.

Clean the docker daemon from all images and containers.

Submit the output for `docker ps -a` and `docker images`

## Solution

1. Clean all containers

       $ docker rm $(docker ps -a -q)
       $ docker ps -a
       CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES

2. Clean all images

       $ docker rmi $(docker images -a -q)
       $ docker images
       REPOSITORY   TAG       IMAGE ID   CREATED   SIZE
