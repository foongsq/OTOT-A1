FROM ubuntu:latest

USER root

RUN apt-get update
RUN apt-get install -y nginx nodejs

RUN rm -v /etc/nginx/nginx.conf
ADD nginx.conf /etc/nginx/
ADD index.html /usr/share/nginx/html
ADD index.html /var/www/html/

RUN echo "daemon off;" >> /etc/nginx/nginx.conf

EXPOSE 3001

CMD service nginx start
