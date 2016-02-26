FROM rails:4.2.5
MAINTAINER Yeghishe Piruzyan ypiruzyan@gmail.com

RUN apt-get update && \
    apt-get install --no-install-recommends -y imagemagick && \
    rm -rf /var/lib/apt/lists/*

RUN mkdir -p /app
WORKDIR /app

ENV RAILS_ENV production
ENV RACK_ENV production
