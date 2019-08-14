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
