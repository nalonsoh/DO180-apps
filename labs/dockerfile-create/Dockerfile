FROM ubi7/ubi:7.7

MAINTAINER Noel Alonso Hernandez <nalonsoh@viewnext.com>
LABEL description="A custom Apache container based on UBI 7"

RUN yum install -y httpd &&\
    yum clean all &&\
    echo "Hello from Dockerfile" > /usr/share/httpd/noindex/index.html

EXPOSE 80

ENTRYPOINT ["httpd", "-D", "FOREGROUND"]






