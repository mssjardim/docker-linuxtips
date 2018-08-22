FROM ubuntu
MAINTAINER Eu (santarelle@gmail.com)
LABEL version="1.0"
LABEL author="Toskao"

RUN apt-get update && apt-get install -y nginx && apt-get clean && rm -rf /var/lib/apt/lists/*

VOLUME /var/www/html/
ADD index.html /var/www/html/
ENV marco lindo

ENTRYPOINT ["/usr/sbin/nginx"]
CMD ["-g", "daemon off;"]
EXPOSE 80

