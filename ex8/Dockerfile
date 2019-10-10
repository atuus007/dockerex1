FROM php:apache-stretch
ARG vhostname=test
RUN echo "<VirtualHost $vhostname:80 >" >> /etc/httpd.conf
RUN echo "SErverName $vhostname " >> /etc/httpd.conf
RUN echo "DocumentRoot /tmp" >> /etc/httpd.conf
RUN echo "</VirtualHost>" >> /etc/httpd.conf

