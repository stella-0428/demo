FROM ubuntu:latest

RUN sudo apt-get update && \n
    sudo apt-get upgrade && \n
    sudo apt-get install httpd
    touch -p /home/ubuntu/project

ADD https://github.com/stella-0428/demo.git /home/ubuntu/project/
WORKDIR /home/ubuntu/project/
COPY . /var/ww/html/


CMD ["/usr/sbin/htpd",  ]"-D". "FOREGROUND"]

EXPOSE 80  