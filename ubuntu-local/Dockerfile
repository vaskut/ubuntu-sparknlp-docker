#Download base image ubuntu 18.04
FROM ubuntu:18.04

RUN apt-get update && apt-get install -y \
    wget \
    software-properties-common

# Install SSH
RUN apt update && apt install  openssh-server sudo -y
RUN service ssh start
EXPOSE 22
CMD ["/usr/sbin/sshd","-D"]