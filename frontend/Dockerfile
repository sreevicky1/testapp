# Deploying a sample webapp frontend
#The commands are the Shell mode commands. These are converted to "Sh -c <command>". In this case shell will be the primary process with PID-1
FROM centos:7
MAINTAINER sree.vicky90@gmail.com
RUN yum -y update
RUN yum -y install httpd
#USER apache
#COPY code/code.zip /var/www/html
ADD code /var/www/html 
ENV BACKENLB=test
EXPOSE 80
COPY config/httpd-foreground /usr/bin
RUN chmod 755 /usr/bin/httpd-foreground
CMD ["httpd-foreground"]





