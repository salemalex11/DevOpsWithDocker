# 1.1 Getting started

## Exercise

Since we already did “Hello, World!” in the material let’s do something else.

Start 3 containers from image that does not automatically exit, such as nginx, detached.

Stop 2 of the containers leaving 1 up.

Submitting the output for docker ps -a is enough to prove this exercise has been done.

# Solution 

1. Start 3 containers

        
        $ docker run -d nginx
        99e14e1a8388949f9589127fece2d8bf1404a6faf37c7cc59877d872885177c3
        $ docker run -d nginx
        976bbcf38fb57b157f96d9a520c159ea4223937fa402f735aad248d06fbd2211
        $ docker run -d nginx
        f90ac54d945f3d16c0651bb8f9e9bf01c10f02beae308c3f92592178f33e5184

2. Stop 2 containers

        $ docker stop f90
        99e
        $ docker stop 99e
        976


3. Use docker ps -a

       $ docker ps -a
       976bbcf38fb5   nginx   "/docker-entrypoint.…"   About a minute ago   Exited (0) 44 seconds ago            vigorous_nobel
       99e14e1a8388   nginx   "/docker-entrypoint.…"   About a minute ago   Exited (0) 51 seconds ago            exciting_banzai
       f90ac54d945f   nginx   "/docker-entrypoint.…"   About a minute ago   Up About a minute           80/tcp   elegant_davinci
