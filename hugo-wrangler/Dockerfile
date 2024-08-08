FROM jenkins/agent:latest-alpine-jdk17

USER root

RUN apk update && \
    apk add --no-cache --repository=https://dl-cdn.alpinelinux.org/alpine/edge/community hugo && \
    apk add --no-cache nodejs npm && \
    rm -rf /var/cache/apk/* && \
    npm install -g wrangler

USER jenkins
