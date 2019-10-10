#ARG version=latest

FROM mysql:latest
ENV MYSQL_ROOT_PASSWORD=12345
ENV MYSQL_PASSWORD=12345
ENV MYSQL_DATABASE=mydb

#RUN mysql -u root -p${MYSQL_ROOT_PASSWORD} -e "CREATE DATABASE mydb"
VOLUME /var/lib/mysql
COPY init.sql /docker-entrypoint-initdb.d
