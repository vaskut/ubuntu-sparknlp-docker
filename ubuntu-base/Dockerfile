#Download base image ubuntu 18.04
FROM rm/ubuntu-local


RUN useradd -rm -d /home/rahulmittal -s /bin/bash -g root -G sudo -u 1000 rahulmittal
RUN  echo 'rahulmittal:password' | chpasswd

CMD ["/usr/sbin/sshd","-D"]