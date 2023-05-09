FROM ubuntu:latest
LABEL name="Ravindra Singh"
LABEL email="ravindrasinghh.me@gmail.com"
ENV UBUNTU_HOME=/var/www/html/
RUN apt-get update -y
ENV DEBIAN_FRONTEND noninteractive	
RUN apt-get -y install tzdata
RUN apt-get install apache2 -y
WORKDIR UBUNTU_HOME
COPY argocd-cicd-setup/script/index.html ${UBUNTU_HOME}
EXPOSE 80
CMD ["apachectl" , "-D","FOREGROUND"]
