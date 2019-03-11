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

docker container run -d --name web -P jboss/wildfly

docker container ls

If you want to change the port:
docker container run -d --name web -p 8080:8080 jboss/wildfly

If you want to remove the container image:
docker container rm -f web

https://github.com/arun-gupta/docker-for-java
copy chapter2 in <username> directory
  
  docker container run -d --name web -p 8080:8080 -v `pwd`/webapp.war:/opt/jboss/wildfly/standalone/deployments/webapp.war jboss/wildfly
  
  curl http://localhost:8080/webapp/resources/persons
  #output:
<collection><person><name>Penny</name></person><person><name>Leonard</name></person><person><name>Sheldon</name></person><person><name>Amy</name></person><person><name>Howard</name></person><person><name>Bernadette</name></person><person><name>Raj</name></person><person><name>Priya</name></person></collection>
 
 
. Dockerfile syntax
. Create a new directory
. Explain build context

```
FROM ubuntu

CMD echo "Hello world" 
  
  
