# list all images
docker image ls

# remove a image
docker image rm <image-id>

# list all containers
docker ps --all

# remove a container 
docker container rm <container-id>

# operation with containers
docker run -it --hostname ds --name <container-name> <image-name> bash
docker pause <container-id/name>
docker unpause <container-id/name>
docker start <container-id/name>
docker stop <container-id/name>
docker kill <container-id/name>
docker rm <container-id/name>
docker inspect <container-id/name>

# commit and tag a container
docker commit <container-name>

# push an image
docker login --username <username>
docker tag <image-name> <username>/<repository-name>:<tag>
docker push <username>/<repository-name>:<tag>
