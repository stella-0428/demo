FROM ubuntu:latest

RUN apt-get update -y && \
    apt-get upgrade -y && \
    apt-get install httpd -y && \
    mkdir -p /home/ubuntu/project

ADD https://github.com/stella-0428/demo.git/ /home/ubuntu/project/
WORKDIR /home/ubuntu/project/
COPY . /var/ww/html/


CMD ["/usr/sbin/httpd",  "-D", "FOREGROUND"]

EXPOSE 80  
