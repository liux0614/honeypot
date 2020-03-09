FROM dorowu/ubuntu-desktop-lxde-vnc:bionic

MAINTAINER Xiang Liu "xiang35@purdue.edu"

#install ssh
RUN apt-get update && apt-get install -y openssh-client

#create a non-root user
RUN useradd -d /home/client -m -s /bin/bash client

RUN echo 'client:client' | chpasswd

ENV USER=client \
    PASSWORD=client

