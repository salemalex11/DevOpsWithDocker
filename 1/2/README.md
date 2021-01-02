# 1.2 Cleanup

## Exercise

We’ve left containers and a image that won’t be used anymore and are taking space, as docker ps -as and docker images will reveal.

Clean the docker daemon from all images and containers.

Submit the output for docker ps -a and docker images

## Solution

$ docker ps -as
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES     SIZE
Alexs-MBP:~ salemalex11$ docker images
REPOSITORY   TAG       IMAGE ID   CREATED   SIZE