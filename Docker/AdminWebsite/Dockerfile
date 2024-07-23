FROM ubuntu:latest
LABEL "Author"="Sujen"
LABEL "Project"="Admin"
ENV DEBIAN_FRONTEND=noninteractive
RUN apt update && apt install git -y
RUN apt install apache2 -y
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
EXPOSE 80
WORKDIR /var/log/apache2
ADD admin.tar.gz /var/www/html
#COPY admin.tar.gz /var/www/html
