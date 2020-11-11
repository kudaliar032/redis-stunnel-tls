# redis-stunnel-tls

### Requirements:
* docker
* docker-compose


### Install

* SSL :
```
cd certs
openssl genrsa -out /etc/stunnel/key.pem 4096
openssl req -new -x509 -key key.pem -out cert.pem -days 1826
```

* site-a
```
cd site-a
docker-compose up -d
```

* On site-b
```
cd site-b
docker-compose up -d
```
