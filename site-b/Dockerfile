FROM alpine:latest

RUN apk update && \
    apk add --no-cache stunnel

ADD ../certs/certs.pem \
    /etc/stunnel/cert.pem

ADD ./stunnel.conf \
    /etc/stunnel/stunnel.conf

EXPOSE 6379
