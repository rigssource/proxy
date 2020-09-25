#download image
FROM nginx:alpine

ENV HTPASSWD='admin:$apr1$GLD1s1oB$AM8YXvUoD0fX6wPNMS0FT0' \
    FORWARD_PORT=80 \
    FORWARD_HOST=web

WORKDIR /opt

RUN apk add --no-cache gettext
#copy configuration files
COPY ./certs/ /etc/nginx/conf.d/
COPY auth.conf auth.htpasswd launch.sh ./

CMD ["./launch.sh"]
