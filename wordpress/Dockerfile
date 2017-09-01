FROM ubuntu_with_php

RUN apt-get install wget -y; \ 
  wget http://wordpress.org/latest.tar.gz; \
  tar xzvf latest.tar.gz; \
  rm -rf latest.tar.gz; \
  cp ~/wordpress/wp-config-sample.php ~/wordpress/wp-config.php; \
  mv wordpress/ /var/www/html/


EXPOSE 80



ENTRYPOINT [ "apachectl","-D","FOREGROUND" ]

