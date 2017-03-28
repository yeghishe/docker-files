FROM alpine:3.5
MAINTAINER Yeghishe Piruzyan ypiruzyan@gmail.com

ARG plugins=awslambda,cors,expires,filemanager,filter,git,hugo,ipfilter,jsonp,jwt,locale,mailout,minify,multipass,prometheus,ratelimit,realip,search,upload

RUN apk update && \
    apk add ca-certificates wget && \
    update-ca-certificates && \
    wget --quiet -O /tmp/caddy.tar.gz "https://caddyserver.com/download/build?os=linux&arch=amd64&features=${plugins}" && \
    mkdir /tmp/caddy && \
    tar -xzf /tmp/caddy.tar.gz -C /tmp/caddy && \
    mv /tmp/caddy/caddy /usr/local/bin && \
    rm -rf /tmp/caddy*

EXPOSE 80 443
WORKDIR /srv

ENTRYPOINT ["/usr/local/bin/caddy"]
CMD ["--log", "stdout"]
