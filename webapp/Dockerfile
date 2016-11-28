FROM ubuntu:14.04
MAINTAINER Chris Trewin <chris.trewin@gmail.com>

RUN apt-get update --fix-missing && apt-get install -y build-essential tar git curl wget dialog net-tools vim

# Install NginX
RUN apt-get install -y nginx

# Switch off the Nginx daemon
RUN echo "daemon off;" >> /etc/nginx/nginx.conf

WORKDIR /

# Start up nginx
ENTRYPOINT ["service","nginx","start"]
