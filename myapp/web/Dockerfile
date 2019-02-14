# My Frist Docker file for create
FROM centos:7
MAINTAINER shan_kelkar@rediffmail.com
RUN yum -y update
RUN yum -y install httpd
ADD code /var/www/html
EXPOSE 80
ENV BACKENDLB=test
CMD ["apachectl","-D","FOREGROUND"]