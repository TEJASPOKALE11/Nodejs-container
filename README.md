This repository contains Dockerfile , package.json and index.js file needed to launch a nodejs container in AWS EC2 instnace .

#To build Dockerfile :

docker build -t nodeimg .

#To check whether image is created using Dockerfile :

docker images

#To launch a container using image of this Dockerfile :

docker run -d -p80:3000 --name nodecontainer nodeimg

#Here the port 80 is port of EC2 instance whereas the port 3000 is port of Nodejs container

#To check whether container is created using image :

docker ps
