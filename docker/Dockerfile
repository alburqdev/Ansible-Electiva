FROM ubuntu:22.04

RUN apt update && \
    apt install -y openssh-server sudo && \
    mkdir /var/run/sshd

# Crear usuario ansible con password "ansible"
RUN useradd -m ansible && echo "ansible:ansible" | chpasswd

# Dar privilegios sudo sin contraseña
RUN echo "ansible ALL=(ALL) NOPASSWD: ALL" >> /etc/sudoers

EXPOSE 22

CMD ["/usr/sbin/sshd", "-D"]
