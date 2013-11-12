# Base
#
# VERSION               0.0.1

FROM       centos:6.4
MAINTAINER Puneet Goyal "puneet@codeignition.co"

RUN yum install openssh-server -y
RUN mkdir /var/run/sshd

RUN echo root:root | chpasswd
RUN service sshd start
RUN service sshd stop

RUN echo "docker run -p 22 -d pungoyal/centos:sshd /usr/sbin/sshd -D" > /.how_to_run

EXPOSE 22

