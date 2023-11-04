# Dockerfile

# Author       : TeknoDroid
# Github       : https://github.com/teknodroid
# Messenger    : https://t.me/Tekn0Droid
# Email        : teknodroidevreni@gmail.com
# Date         : 08-09-2022
# Main Language: Python

# Download and import main images

# Operating system
FROM debian:latest
# Main package
FROM python:3

# Author info
LABEL MAINTAINER="https://github.com/teknodroid/TeknoPhisher"

# Working directory
WORKDIR /TeknoPhisher/
# Add files 
ADD . /TeknoPhisher

# Installing other packages
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install python3-pip php openssh-client -y
RUN pip3 install -r files/requirements.txt --break-system-packages
RUN apt-get clean

# Main command
CMD ["python3", "teknophisher.py", "--noupdate"]

## Wanna run it own? Try following commnads:

## "sudo docker build . -t teknodroid/teknophisher:latest", "sudo docker run --rm -it teknodroid/teknophisher:latest"

## "sudo docker pull teknodroid/teknophisher", "sudo docker run --rm -it teknodroid/teknophisher"
