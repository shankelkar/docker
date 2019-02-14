#This my Second nginx docker file
FROM ubuntu:18.04
MAINTAINER shan_kelkar@rediffmail.com
RUN apt-get -y update
RUN apt-get -y install tzdata
ENV TZ = "US"
ADD config /opt
RUN apt-get -y install `cat /opt/packages`
ADD code /var/www/html
EXPOSE 80
CMD ["nginx","-g","daemon off;"]