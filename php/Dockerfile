FROM ubuntu_with_apache

RUN apt-get update && apt-get install -y \
php libapache2-mod-php php-mcrypt php-mysql  

EXPOSE 80



ENTRYPOINT [ "apachectl","-D","FOREGROUND" ]

