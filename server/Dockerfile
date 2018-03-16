# Docker 
FROM amazonlinux:2
MAINTAINER satoshi.kanazawa

RUN yum -y localinstall https://dev.mysql.com/get/mysql57-community-release-el7-11.noarch.rpm
RUN yum -y install mysql-community-server
RUN systemctl enable mysqld.service

# edit prompt
RUN echo 'PS1="[\u@amazonlinux2 \W]$ "' >> ~/.bashrc

# start service
CMD ["/sbin/init"]
