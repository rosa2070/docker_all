FROM ubuntu:20.04
RUN apt update
RUN apt-get install -y nginx
COPY ./index.html /var/www/html
COPY ./1.jpg /var/www/html
ENTRYPOINT [ "nginx", "-g", "daemon off;" ]
EXPOSE 80

# docker build . -t mynginx
# docker run -d -p 7777:80 --name mycontainer mynginx