FROM registry.apps.ocp45.lab.kx.com/rockylinux:9
RUN  echo 'root:root123' | chpasswd
RUN useradd artak -s /bin/bash && useradd bob -s /bin/bash
RUN  echo 'artak:artak123' | chpasswd 
RUN dnf install sudo unzip git -y
RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" && unzip awscliv2.zip && ./aws/install
