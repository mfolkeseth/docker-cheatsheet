# Docker cheat sheet

## Remove active containers
    $docker rm $(docker ps -aq)

## Docker host IP
    $echo $DOCKER_HOST

## Run image locally
    $docker run -itP --expose 8080 -p <desired port>:8080 --name <container name> <image id> npm start

## Run local image
    http://DOCKER_HOST:<chosen port>
