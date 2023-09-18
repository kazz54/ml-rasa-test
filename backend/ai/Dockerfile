FROM ubuntu
WORKDIR /ai

RUN apt-get update
RUN apt-get -y install tzdata
#RUN apt-get -y install apache2
RUN apt -y install python3.10 python3.10-venv supervisor
#RUN echo "Dockerfile Test on Apache2" > /ai/index.html
ADD supervisord.conf /etc/supervisor/supervisord.conf
COPY . /ai/
CMD ["/usr/bin/supervisord"]

#RUN echo "Dockerfile Test on Apache2" > /ai/index.html

#CMD ["/ai/", "-D", "FOREGROUND"]