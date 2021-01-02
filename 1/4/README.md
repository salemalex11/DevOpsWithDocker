# 1.4

## Exercise

Now that we’ve warmed up it’s time to get inside a container while it’s running!

Start image `devopsdockeruh/exec_bash_exercis`e, it will start a container with clock-like features and create a log. Go inside the container and use `tail -f ./logs.txt` to follow the logs. Every 15 seconds the clock will send you a “secret message”.

Submit the secret message and command(s) given as your answer.

## Solution

1. Start the container
                  
        $ docker run -d -it devopsdockeruh/exec_bash_exercise
         83a39102ad6b63be6c95e5edafd8e254ea4c7bcf34992db62af0fbd4208fd923
    
2. Go inside the container 

       $ docker exec -it 83 bash
       root@83a39102ad6b:/usr/app#


3. Use tail -f ./logs.txt to follow the logs

       root@83a39102ad6b:/usr/app# tail -f ./logs.txt
       Sat, 02 Jan 2021 22:06:31 GMT
       Secret message is:
       "Docker is easy"
