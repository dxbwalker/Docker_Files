# Dockerfile based on the latest CentOS 7 image and will start Apache in each container
FROM centos:latest
MAINTAINER crok_cy@yahoo.com

RUN yum update -y
RUN yum install -y httpd net-tools

RUN echo "This is custom index file building during the image" > /var/www/html/index.html

EXPOSE 80
ENTRYPOINT apachectl "-DFOREGROUND"

#Test
