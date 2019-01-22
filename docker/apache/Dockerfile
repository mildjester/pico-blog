FROM amazonlinux:2017.03-with-sources

RUN yum update -y \
 && yum install -y vim httpd hp php-devel php-pdo php-xml php-mbstring \
 && cp -p /usr/share/zoneinfo/Japan /etc/localtime

CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]
