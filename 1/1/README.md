# 1.1 Getting started

## Exercise

Since we already did “Hello, World!” in the material let’s do something else.

Start 3 containers from image that does not automatically exit, such as nginx, detached.

Stop 2 of the containers leaving 1 up.

Submitting the output for docker ps -a is enough to prove this exercise has been done.

# Solution 

    $ docker ps -a
    CONTAINER ID   IMAGE     COMMAND                  CREATED          STATUS                     PORTS     NAMES
    99da55ffc681   nginx     "/docker-entrypoint.…"   32 seconds ago   Exited (0) 3 seconds ago             quizzical_hoover
    476c405e0dbe   nginx     "/docker-entrypoint.…"   33 seconds ago   Exited (0) 3 seconds ago             brave_galileo
    f78b0cf19669   nginx     "/docker-entrypoint.…"   35 seconds ago   Up 34 seconds              80/tcp    compassionate_taussig
