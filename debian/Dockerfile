FROM debian:jessie
MAINTAINER Yeghishe Piruzyan ypiruzyan@gmail.com

RUN apt-get update && \
    apt-get install --no-install-recommends -y curl wget jq zip unzip htop telnet build-essential python && \
    rm -rf /var/lib/apt/lists/*
