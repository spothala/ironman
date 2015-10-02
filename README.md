# ironman
This creates different versions of ironman docker images

# Following command creates file at ~/.docker/config
$ docker login

$docker-machine env default
$ docker-machine restart default      # Restart the environment
$ eval $(docker-machine env default)  # Refresh your environment settings

$ packer build <>.json

# How to RUN docker images
$ docker run -d -i -p 8080:80 --privileged=true --name nginx_v1 autobot/ironman:v1 /bin/bash -c '/usr/bin/supervisord'
$ docker exec -it nginx_v1 /bin/bash
