FROM registry.access.redhat.com/ubi7/ubi:7.9-641.1645812159
MAINTAINER Chandra Prakash <cprakash1804@qcsdclabs.com>
USER root
LABEL description="A base image for JBOSS 7.4 on UBI7.9"
RUN yum install -y httpd  && \
    yum clean all
RUN echo "A base image for JBOSS 7.4 on UBI7.9" > /var/www/html/index.html 
EXPOSE 80
CMD ["httpd", "-D", "FOREGROUND"]
