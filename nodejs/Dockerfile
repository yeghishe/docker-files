FROM skupit/base:v1
MAINTAINER Yeghishe

RUN curl -sL https://deb.nodesource.com/setup_0.12 | sudo bash - && apt-get update && sudo apt-get install -y nodejs=0.12.7-1nodesource1~trusty1
RUN npm install -g coffee-script forever
