# Docker Basics:
1. Getting started with docker
```
docker run [image]
```
2. To start with a default command. The command should exist in the container. This default command cannot be changed later.
```
docker run [image] [command]
```
3. Listing running containers
```
docker ps
```
4. List of all containers ever created
```
docker ps --all
```
5. ```run``` command creates and starts a container. You can do it seperately.
```
docker create [image] 
docker start -a [id]
````
  Here ```-a ```  logs output to the terminal. By default, ```run``` logs output.  
  
6. To completely remove all stopped containers
```
docker system prune
```
7. To get logs from a container. Doesn't restart container.
```
docker logs [id]
```
8. To stop a container. This command gives the processes inside the container some time (SIGTERM) to do some clean up eg. produce logs, etc.
```
docker stop [id]
```
9. To kill a container. Container is killed instantly without any time to do clean up.
```
docker kill [id]
```
10. Executing commands in running containers.
```
docker exec -it [id] [command]
```
11.  ```-it``` flag is actually combination of two seperate flags. ```-i``` connects terminal to STDIN, STDOUT, and STDERR of the container, and ```-t``` beautfies outputs.  
  
12. Getting a shell in a Container
```
docker exec -it [id] sh
```
13. Starting with a shell, eg:
```
docker run -it [image] sh
```
14. 


