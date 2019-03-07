# docker_for_java_developers
Docker:
=====
Build docker image
Ship docker hub
Run docker container

(J,E,W)AR —> WORA = write Once, Run Anywhere
Image —> PODA = Package Once, Deploy Anywhere

App1
Bins/Libs
MacOS
—Hyoervisor—
—Host OS—
---Infrastructure—

  
App1
Bins/Libs
Docker Engine
OS
Infrastructure

Docker WorkFlow:
Client:                        Docker Hsot                            Registry
Docker build             Docker daemon
Docker pull                containers    Images 
Docker run 
 

Once you installed the docker.

docker-machine —version

docker-machine create -d virtualbox myhost

If you are facing issues while installing Virtualbox.
Please follow below link
http://biercoff.com/how-to-fix-docker-machine-installation-on-mac-os-x/
   
 env | grep DOCKER
 
 docker-machine env myhost
 
#Run below command to configure your shell:
eval $(docker-machine env myhost5)
env | grep DOCKER

