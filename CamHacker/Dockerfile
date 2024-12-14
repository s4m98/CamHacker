# Dockerfile

# Script       : CamHacker
# Author       : Mohit Sambharwal
# Github       : https://github.com/s4m98
# Date         : 12-12-2024
# Main Language: Shell

# Download and import main images

# Operating system
FROM debian:latest

# Author info
LABEL MAINTAINER="https://github.com/s4m98/CamHacker"

# Working directory
WORKDIR /CamHacker/
# Add files 
ADD . /CamHacker

# Installing other packages
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install curl unzip wget -y
RUN apt-get install --no-install-recommends php -y
RUN apt-get clean

# Main command
CMD ["./ch.sh", "--no-update"]

## Wanna run it own? Try following commnads:

## "sudo docker build . -t s4m98/camhacker:latest", "sudo docker run --rm -it s4m98/pyphisher:latest"

## "sudo docker pull s4m98/camhacker", "sudo docker run --rm -it s4m98/camhacker"
