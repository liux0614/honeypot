FROM dorowu/ubuntu-desktop-lxde-vnc:bionic

MAINTAINER Xiang Liu "xiang35@purdue.edu"

#install ssh
RUN apt-get update && apt-get install -y openssh-server rsyslog vim gedit

#create a non-root user
#RUN useradd --group sudo -d /home/honeypot -m -s /bin/bash honeypot

RUN echo "root:Docker" | chpasswd

ENV USER=root \
    PASSWORD=Docker

COPY 50-default.conf /etc/rsyslog.d/

#RUN sudo service ssh start
#RUN sudo service rsyslog start



