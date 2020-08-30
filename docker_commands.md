# INSTALLTION

   56  sudo apt-get remove docker docker-engine docker.io containerd runc
   
   57  sudo apt-get install     apt-transport-https     ca-certificates     curl     gnupg-agent     software-properties-common
   
   58  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
   
   59  sudo apt-key fingerprint 0EBFCD88
   
   60  sudo add-apt-repository    "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   61     $(lsb_release -cs) \
   62     stable"
   
   63  sudo apt-get update
   
   64  sudo apt-get install docker-ce docker-ce-cli containerd.io
   
   65  apt-cache madison docker-ce
   
   66  docker -v
   
  ## VERIFICATION
   67  docker run busybox ech 'hi there'
   
 ## COMMANDS
   68  sudo docker run busybox ech 'hi there'
   
   69  sudo docker run busybox echo 'hi there'
   
   70  sudo docker run busybox echo 'hi there jnjn'
   
   71  sudo docker ps
   
   72  sudo docker run busybox ping www.google.com
   
   73  docker ps
   
   74  sudo docker ps
   
   75  sudo docker exec -it a707008cae13 redis-cli
   
   76  docker images
   
   77  sudo docker images
   
   78  docker ps
   79  sudo docker ps

   83  sudo docker exec -it a707008cae13 sh
   84  sudo docker run -it busybox sh
   
   # build image
   67  cd simpleweb/
   68  ls
   69  docker build .
   
 docker images 
 
 docker run 34735fdde64b -p 8080:8080
 
 docker run -p 8080:8080 34735fdde64b
 
 docker exec -it 34735fdde64b sh
 
 docker exec -it 48ee4c7a2741 sh
   

