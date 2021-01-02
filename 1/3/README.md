# 1.3 Hello Docker Hub

## Exercise

Start image devopsdockeruh/pull_exercise with flags -it like so: docker run -it devopsdockeruh/pull_exercise. It will wait for your input. Navigate through docker hub to find the docs and Dockerfile that was used to create the image.

Read the Dockerfile and/or docs to learn what input will get the application to answer a “secret message”.

Submit the secret message and command(s) given to get it as your answer.

## Solution

    $ docker run -it devopsdockeruh/pull_exercise
    Give me the password: basics
    You found the correct password. Secret message is:
    "This is the secret message"
