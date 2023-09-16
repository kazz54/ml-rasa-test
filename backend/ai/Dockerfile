FROM ubuntu

RUN apt-get update
RUN apt-get -y install tzdata
RUN apt-get -y install apache2
RUN echo "Dockerfile Test on Apache2" > /var/www/html/index.html

CMD ["/usr/sbin/apachectl", "-D", "FOREGROUND"]