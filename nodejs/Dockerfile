FROM yeghishe/debian:jessie
MAINTAINER Yeghishe Piruzyan ypiruzyan@gmai.com

RUN curl -sL https://deb.nodesource.com/setup_0.12 | bash - && \
    apt-get update && \
    apt-get install --no-install-recommends -y nodejs=0.12.7-1nodesource1~jessie1 && \
    rm -rf /var/lib/apt/lists/*
RUN npm install -g coffee-script forever
