# Simple Web Server Dockerfile
FROM ubuntu:15.04
RUN apt-get update && apt-get install -y \
        apache2 \
        apache2-utils \
        vim \
        && apt-get clean \
        && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
EXPOSE 80
VOLUME /data
ENTRYPOINT ["apache2ctl"]
CMD ["-D", "FOREGROUND"]
