# learning-docker

## Comands 

    docker run nginx
Pull the image if its not in local and start the container

    docker ps
list all runing containers

    docker ps -a 
runing + stoped 

    docker stop <c-id or c-name>
stop the runing container 

    docker rm <c-id or c-name>
remove stopped or exited container

    docker images
list of all images

    docker rmi <image-name>
remove image (no c runing using that image) 

    docker pull <image-name>
pull docker image from docker artifact

    docker exac
enter into docker container

    docker run -d nginx
Run c in bg and return to console 

    docker attach nginx
attache again to c with -d
    docker run --name <name> -d -p 80:80 image 

    docker run -it 
interactive mode 

underlaing host where docker is installed is docker host/docker engine

    docker run -p 80:5000 webapp

5000 from container is accesible on 80 in docker host.

    docker run -v /opt/datadir:/var/lib/mysql mysql
mount vlue to container from docker host 

    docker inspect <c-name>
    docker logs <c-name>

# Adv

    docker network create --driver bridge \
    --subnet 182.8.9.9/16
    cosyome-isolation