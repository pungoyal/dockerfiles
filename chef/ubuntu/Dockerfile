# Base
#
# VERSION               0.0.1

FROM       ubuntu
MAINTAINER Puneet Goyal "puneet@codeignition.co"

RUN apt-get install aptitude wget screen curl -y
RUN wget https://opscode-omnibus-packages.s3.amazonaws.com/ubuntu/12.04/x86_64/chef-server_11.0.8-1.ubuntu.12.04_amd64.deb
RUN dpkg -i chef-server_11.0.8-1.ubuntu.12.04_amd64.deb

