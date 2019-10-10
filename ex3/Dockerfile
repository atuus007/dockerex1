FROM httpd:2.4
ENV APACHE_DOCUMENT_ROOT=/home/www/docroot
ENV APACHE_USER=www

#RUN mkdir -p ${APACHE_DOCUMENT_ROOT}

RUN useradd --uid 1000 www
COPY httpd.conf conf/httpd.conf

#User www
#Group www
#Documentroot "/home/www/docroot"
#<Directory>
#	Allow from all
#</directory



#RUN adduser www
#RUN usermod -u 1000 www
#RUN usermod -aG root ${APACHE_USER}
#USER ${APACHE_USER}

RUN rm htdocs/index.html
RUN echo "ServerSignature Off" >> conf/httpd.conf
RUN echo "ServerTokens Prod" >> conf/httpd.conf

VOLUME ${APACHE_DOCUMENT_ROOT}
