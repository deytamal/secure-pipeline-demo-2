FROM httpd:latest
COPY index.html /usr/local/apache2/htdocs/
COPY security.conf /usr/local/apache2/conf/extra/security.conf
RUN sed -i 's/^#LoadModule headers_module/LoadModule headers_module/' /usr/local/apache2/conf/httpd.conf \
 && echo 'Include conf/extra/security.conf' >> /usr/local/apache2/conf/httpd.conf
