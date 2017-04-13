## install docker on ubuntu: 
`$ curl -fsSL https://get.docker.com/ | sh`
## change user group, dont need to sudo every time
`$ sudo usermod -aG docker $(whoami)`
## Build an image on a Dockerfile
`$ docker build -t TAGNAME DOCKER_FILE_PATH`
## check build好的image
`$ docker images`
## login docker hub
`$ docker login`
## push image to your repo on docker hub
`$ docker push`
## pull image
`$ docker pull IMAGE_NAME`

docker-compose up --build
# stop all containers:       
`$ docker stop $(docker ps -a -q)`

# remove all containers:     
`$ docker rm $(docker ps -a -q)`

# remove all docker images:  
`$ docker rmi $(docker images -q)`