FROM ubuntu:latest
ENV TZ=Europe/Kiev
ENV DEVOPS="Alex Chekh"
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone \
	    &&apt-get update && apt-get install -y apache2
EXPOSE 80
RUN echo $DEVOPS > /var/www/html/index.html  
CMD apachectl -D FOREGROUND
