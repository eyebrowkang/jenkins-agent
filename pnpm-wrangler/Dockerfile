FROM jenkins/agent:latest-alpine-jdk17

USER root

RUN apk update && \
    apk add --no-cache nodejs npm && \
    npm install -g pnpm wrangler && \
    rm -rf /var/cache/apk/* /root/.npm/*

USER jenkins
