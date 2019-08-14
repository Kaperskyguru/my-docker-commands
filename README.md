# my-docker-commands
Curated list of my popular docker commands

## List Docker CLI commands
```bash 
docker
docker container --help
```

## Display Docker version and info
```bash
docker --version
docker version
docker info
```

## Execute Docker image
```bash
docker run hello-world
```

## List Docker images
```bash
docker image ls
```

## List Docker containers (running, all, all in quiet mode)
```bash
docker container ls
docker container ls --all
docker container ls -aq
```

## Build an Image
```bash
docker build --tag=friendlyhello .
```

## Running the Image
```bash
docker run -p 4000:80 friendlyhello
```

## To stop an Image
```bash
docker container stop CONTAINER_ID
```


# SHARING YOUR IMAGE IN DOCKERHUB

## To Login into docker hub
```bash
docker login
```

## Tag the image
```bash
docker tag image username/repository:tag
e.g.
docker tag friendlyhello kaperskyguru/get-started:v2
```

## Publish the image
```bash
docker push username/repository:tag
```

## Pull and run the image from the remote repository
```bash
docker run -p 4000:80 username/repository:tag
```

## Remove containers and images
```bash
docker container rm <hash>
docker container rm $(docker container ls -a -q)         # Remove all containers

docker image rm <image id>            # Remove specified image from this machine
docker image rm $(docker image ls -a -q)   # Remove all images from this machine
```
