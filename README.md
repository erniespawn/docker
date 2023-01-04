# docker
docker tutorial

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


