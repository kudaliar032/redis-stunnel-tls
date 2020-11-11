FROM alpine:latest

RUN apk update && \
    apk add --no-cache stunnel

ADD ./stunnel.conf /stunnel.conf

EXPOSE 6379
