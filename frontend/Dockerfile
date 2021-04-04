FROM node:14.16-alpine

WORKDIR /app

ENV LANG C.UTF-8
ENV TZ Asia/Tokyo

RUN apk update && \
    apk upgrade && \
    npm install && \
    # バージョン指定をしないと'npx create-nuxt-app'で'non-empty directory'エラーが発生
    npm install -g create-nuxt-app@2.15.0

ADD . /app
