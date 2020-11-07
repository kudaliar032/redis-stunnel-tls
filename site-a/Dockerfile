FROM redis:alpine

RUN apk update && \
    apk add --no-cache stunnel

COPY private.pem /

RUN chmod 640 /private.pem

ADD ./stunnel.conf /stunnel.conf

EXPOSE 6379
