# dockerfiles

Contains dockerfiles for Data Science work.

## Commands

### docker images

View a list of images.


### docker ps -a

View a list of all containers (both running and not running)

### docker stop <container id>

Stops one or more running containers.

### docker kill $(docker ps -q)

Kill all running containers.

### docker rm \<container id\>

Removes stopped container

### docker rm $(docker ps -a -q)

Delete all stopped containers

### docker rm \<image id\>

Removes image

### docker rmi $(docker images -q)

Delete all images

### docker pull

Pull a pre-built image from Docker Hub without needing to define and configure it.

### docker build

Build a Docker image from a Dockerfile.  Use -t to label the image, e.g.: `docker build -t base_python3 .`

### docker run

Run a docker container based on an image.  Use `-it bash` with this command to run bash from the container.  E.g.: `docker run base_python3 -it bash`

`-v` : map local directory to location on the container:  `docker run -v ~/workspace/data:/home/app`
