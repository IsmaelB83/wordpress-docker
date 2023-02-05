# wordpress-docker
Docker-compose.yml descriptor to start a wordpress site 

# To start the site just:
$ git clone https://github.com/IsmaelB83/wordpress-docker.git
$ cd wordpress-docker/
$ wordpress-docker/sudo docker-compose up

# To check running containers
$ docker container list
CONTAINER ID   IMAGE                   COMMAND                     CREATED          STATUS                  PORTS                                                    NAMES
0f674a2baf78   wordpress:latest        "docker-entrypoint.s…"      36 hours ago     Up About a minute       0.0.0.0:4282->80/tcp, :::4282->80/tcp                    wordpresscontainer
950b50249e34   phpmyadmin/phpmyadmin   "/docker-entrypoint.…"      36 hours ago     Up About a minute       0.0.0.0:4283->80/tcp, :::4283->80/tcp                    phpmyadmincontainer
d86d384d185b   mysql:5.7               "docker-entrypoint.s…"      36 hours ago     Up About a minute       33060/tcp, 0.0.0.0:4208->3306/tcp, :::4208->3306/tcp     mysqlcontainer

# To delete containers
$ docker container prune
WARNING! This will remove all stopped containers.
Are you sure you want to continue? [y/N] y
Deleted Containers:
0f674a2baf786227f3a90cd9164e84fa9ea788026dfd2b64507e24635a0c09dc
950b50249e34741235933324848f64d9334316d6d2ddfb61f3bd3da2b17fd487
d86d384d185b67c1d338d8804f7b5ec98394e46afaa0977382c2a5d68cf4f813
