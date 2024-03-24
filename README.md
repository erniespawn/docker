# docker
docker tutorial

## Create docker debian12 with network and full privileged

```
How docker with Debian12. 

cd debian-strongswan-latest
docker build -t docker-debian/strongswan:latest . 
docker run -it --net=bridge --privileged docker-debian/strongswan:latest

```

---







Show current running containers
- docker ps

Show all containers
- docker ps -a
- docker container ls -a 

Show images
- docker images 

Pull any container
- docker pull alpine
- docker pull ubuntu
- docker pull debian

Create a Dockerfile 
- vim Dockerfile

Build docker image
- docker build . -t myubuntu

Run the container
- docker run -it myubuntu

Remove stopped containers
- docker rmi [IMAGE ID]

Remove images
- docker images
- docker rm [REPOSITORY] or docker rm [IMAGE ID] or docker rm [REPOSITORY:TAG]


How to host website in docker?

https://github.com/docker-library/docs/tree/master/httpd   



