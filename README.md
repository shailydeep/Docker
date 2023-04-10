# Docker
######### HOW TO INSTALL DOCKER AND MANAGE DOCKER IMAGES (DEAMON IMAGE) #######
#PACKAGE NAME > docker-ce
#SERVICE NAME > docker.service
#DEFAULT REGISTRY FROM DOCKERHUB > docker.io
#REDHAT REGISTRY   > quay.io
SOLUTION >

 1  yum install -y yum-utils
 2   yum-config-manager     --add-repo     https://download.docker.com/linux/centos/docker-ce.repo
 3  ls /etc/yum.repos.d/
 4  yum -y install docker-ce
 5  systemctl enable --now docker
###  HOW TO MANAGE DOCKER IMAGES### 

 1  docker info                                   [TO LIST INFORMATION ABOUT DOCKER]
 2  docker version                                [TO CHECK VERSION INFO] 
 3  docker --version                              [TO CHECK VERSION] 
 4  docker images                                 [TO LIST DOCKER IMAGES]
 5  docker search REGISTRY/IMAGENAME              [TO SEARCH DOCKER IMAGE FROM GIVEN REGISTRY]
 6  docker search IMAGENAME                       [TO SEARCH IMAGE IN DEFAULT REGISTRY]
 7  docker pull IMAGENAME                         [TO PULL IMAGE FROM DEFAULT REGISTRY]                                                                               
 8  docker pull REGISTRY/IMAGENAME                [TO PULL DOCKER IMAGE FROM GIVEN REGISTRY]
 9  docker pull ubuntu:22.04                      [TO PULL IMAGE:TAG ]
10  docker tag IMAGEIDNO NAME:latest              [TO CHANGE NAME:TAG EX- docker tag imageidno deep:latest] 
11  docker rmi mysql:latest                       [TO REMOVE DOCKER IMAGE:TAG]
12  docker rmi TAGNAME                            [TO REMOVE WITH TAGNAME]
13  docker rmi -f IMAGEIDNO                       [TO REMOVE WITH IMAGEIDNO]
14  docker save IMAGEIDNO -o backup.tar           [TO TAKE BACKUP OF DOCKER IMAGE]
15  ls                                        
16  docker load -i backup.tar                     [TO EXTRACT BACKUP OF DOCKER IMAGE]
17  docker images                                  
        
   
