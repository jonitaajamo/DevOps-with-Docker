FROM ubuntu:16.04 

WORKDIR /1.4
RUN apt-get update && apt-get install -y curl 
CMD read website; sleep 3; curl http://$website;  
