# Docker

# To Build own ssh image

     sudo docker build -t veeru .

# To Run your ssh container ditached mode     
     
     sudo docker run -d -P --name ssh_serv veeru
     
# To start and stop container 
     sudo docker start ssh_serv
     
     sudo docker stop ssh_serv
     
# To check binding port of container 
    sudo  docker ps -a

# To ssh login to your container
      1 first check iaddress of docker bridge ip 
           ifconfig  docker0
      2 run below connamd
           ssh root@dockerbridgeip 
      
