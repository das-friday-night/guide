## install docker on ubuntu: 
`$ curl -fsSL https://get.docker.com/ | sh`

## change user group, dont need to sudo every time
`$ sudo usermod -aG docker $(whoami)`

## Build an image on a Dockerfile
`$ docker build -t TAG_NAME DOCKER_FILE_PATH`

## check build好的image
`$ docker images`

## run image on Docker
`$ docker run --name APP_NAME -p PORT_MAPPING -d IMAGE_NAME`
example: 
`$ docker run --name tiny -p 3000:3000 -d tinyurl`

---
## login docker hub
`$ docker login`

## push image to your repo on docker hub
`$ docker push`

## pull image
`$ docker pull IMAGE_NAME`

---
# stop all containers:       
`$ docker stop $(docker ps -a -q)`

# remove all containers:     
`$ docker rm $(docker ps -a -q)`

# remove all docker images:  
`$ docker rmi $(docker images -q)`
