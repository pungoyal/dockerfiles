# Base
#
# VERSION               0.0.1

FROM       ubuntu:12.10
MAINTAINER Puneet Goyal "puneet@codeignition.co"

RUN apt-get update
RUN apt-get install aptitude -y
RUN apt-get install openssh-server -y
RUN mkdir /var/run/sshd

RUN echo root:root | chpasswd
RUN echo "docker run -p 22 -d pungoyal/ubuntu:sshd" > /.how_to_run

EXPOSE 22

ENTRYPOINT ["/usr/sbin/sshd", "-D"]

