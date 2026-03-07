FROM amazonlinux:latest
RUN yum install httpd -y
COPY index.html /var/www/html/index.html
CMD ["/usr/sbin/httpd", "-DFOREGROUND"]
EXPOSE 80
