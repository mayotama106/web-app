FROM node:12.13-alpine

RUN yarn global add mkdirp@1.0.3
RUN mkdir /app
WORKDIR /app

RUN apk update && \
    apk upgrade && \
    apk add git 
RUN yarn global add nuxt create-nuxt-app && \
    yarn global add firebase-tools

ENV LANG C.UTF-8
ENV TZ Asia/Tokyo
ENV HOST 0.0.0.0
EXPOSE 3000