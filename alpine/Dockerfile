FROM lysender/node:alpine
MAINTAINER Leonel Baer <leonel@lysender.com>

RUN apk add --no-cache supervisor && \
    npm -g install socket.io express aws-sdk

VOLUME ["/var/log/supervisor"]
EXPOSE 4040
CMD ["supervisord", "-n"]

