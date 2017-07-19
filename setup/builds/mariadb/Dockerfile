#docker build .
FROM mariadb

MAINTAINER Elias Barbosa <info@eb8.com>

RUN mkdir -p /root/mysql

RUN apt-get -y update
RUN apt-get -y --fix-missing install cron
RUN apt-get -y --fix-missing install rsync
RUN apt-get -y --fix-missing install nano

# RUN echo '* * * * * root /usr/bin/rsync -a /var/lib/mysql /root/mysql' >> /etc/crontab
RUN echo '* * * * * root A=/var/www/html && B=/html && /usr/bin/rsync -azu $A $B && /usr/bin/rsync -azu $B $A' >> /etc/crontab