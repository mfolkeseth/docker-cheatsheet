# Docker cheat sheet

## Remove active containers
**Remove all**

    $docker rm $(docker ps -aq)

**Remove single**

    $docker rm <container id>
    
## Remove images
**Remove all**

    $docker rmi $(docker images -aq)

**Remove single**

    $docker rmi <image id>

## Docker host IP
    $echo $DOCKER_HOST

## Run image locally
    $docker run -itP --expose 8080 -p <desired port>:8080 --name <container name> <image id> npm start

## Run local image
    http://DOCKER_HOST:<chosen port>
