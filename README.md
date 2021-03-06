## Creating the Docker images
```
#!bash

# Switch to one of the directories (e.g. dev-base) and run the docker build command:
$ cd dev-base
$ docker build -t ${PWD##*/} .
```
![Docker Images](https://github.com/logikburg/dockrant/blob/master/docker_images.png)

## Running an instance
```
#!bash

# Assuming $GOPATH has been set and using the dev-golang instance:
$ docker run --rm -it -v ${GOPATH}:/home/godev/gocode dev-golang
```
![Docker Images](https://github.com/logikburg/dockrant/blob/master/docker_running.png)
