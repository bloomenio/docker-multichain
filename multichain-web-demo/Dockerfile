FROM php:7.0-apache

ARG CHAINNAME
ARG RPC_PORT
ARG RPC_USER
ARG RPC_PASSWORD
ARG MASTER_NODE

RUN apt-get update && apt-get install -y \
  git 

RUN cd /var/www/html

RUN git clone https://github.com/worldline-spain/multichain-web-demo.git

RUN echo "default.name="${CHAINNAME} >> /var/www/html/multichain-web-demo/config.txt
RUN echo "default.rpchost="${MASTER_NODE} >> //var/www/html/multichain-web-demo/config.txt
RUN echo "default.rpcport="${RPC_PORT} >> //var/www/html/multichain-web-demo/config.txt
RUN echo "default.rpcuser="${RPC_USER} >> //var/www/html/multichain-web-demo/config.txt
RUN echo "default.rpcpassword="${RPC_PASSWORD} >> //var/www/html/multichain-web-demo/config.txt

 