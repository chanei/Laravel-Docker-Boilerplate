# Laravel-Docker-Boilerplate
Laravel 7 Docker Boilerplate with running the Dockerfile only

## Building the docker image for the laravel project
- ```docker build -t laravel_project .``` - replace laravel_project with the preferred name of your image. <b>Don't forget the ```.``` at the end of the command
- ```docker run -p 80:80 laravel_project``` - 80 is the port that is being exposed in the dockerfile

## Useful Docker Commands

- ```docker``` - shows all the docker commands
- ```docker version``` - shows docker related versions
- ```docker info``` - shows information about number of containers running and images
- ```docker ps``` or ```docker container ls``` - shows list of containers
- ```docker container ls -a``` - shows list of running containers
- ```docker container rm container_id``` - removes a container (replace container_id with the actual container id)
- ```docker images``` - shows available created images
- ```docker image rm image_id``` - removes a docker image of specified image_id
- ```docker rm $(docker ps -aq) -f``` - removes all containers where the ```-f``` flag forces to remove even the running containers
- ```docker rmi -f $(docker images -a -q)``` - removes all images
- ```docker image build -t docker_hub_username/your_image_name``` - send your image to dockerhub account
- ```docker push docker_hub_username/your_image_name```
- ```docker login``` - authentication

<p>To view the full list of docker commands, Check the 
<a href="https://docs.docker.com/">Docker documentation</a></p>
