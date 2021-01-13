FROM node:lts-alpine

WORKDIR /app

RUN apk update && \
    apk install git vim bash && \
    npm install -g npm && \
    npm install -g vue-cli