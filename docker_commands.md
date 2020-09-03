# INSTALLTION

 sudo apt-get remove docker docker-engine docker.io containerd runc

 sudo apt-get install     apt-transport-https     ca-certificates     curl     gnupg-agent     software-properties-common

 curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

 sudo apt-key fingerprint 0EBFCD88

 sudo add-apt-repository    "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
    $(lsb_release -cs) \
    stable"

 sudo apt-get update

 sudo apt-get install docker-ce docker-ce-cli containerd.io

 apt-cache madison docker-ce

 docker -v
   
## VERIFICATION

docker run busybox ech 'hi there'
   
 ## COMMANDS
 
sudo docker run busybox ech 'hi there'

sudo docker run busybox echo 'hi there'

sudo docker run busybox echo 'hi there jnjn'

sudo docker ps

sudo docker run busybox ping www.google.com

docker ps

sudo docker ps

sudo docker exec -it a707008cae13 redis-cli

docker images

sudo docker images

docker ps
sudo docker ps

sudo docker exec -it a707008cae13 sh

sudo docker run -it busybox sh
   

# build image

cd simpleweb/

ls

docker build .
   
docker images 
 
docker run -p 8080:8080 34735fdde64b
 
docker exec -it 34735fdde64b sh
 
docker exec -it 48ee4c7a2741 sh   

