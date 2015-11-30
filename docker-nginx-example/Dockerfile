FROM ubuntu:14.04.3

RUN apt-get install -y nginx
RUN echo "daemon off;" >> /etc/nginx/nginx.conf
EXPOSE 80
CMD ["nginx"]
