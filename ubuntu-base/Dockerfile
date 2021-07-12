FROM vaskut/ubuntu-local

ENV USERNAME 'vaskut'
ENV PASSWORD 'password'

RUN useradd -rm -d /home/${USERNAME} -s /bin/bash -g root -G sudo -u 1000 ${USERNAME}
RUN  echo ${USERNAME}:${PASSWORD} | chpasswd

CMD ["/usr/sbin/sshd","-D"]