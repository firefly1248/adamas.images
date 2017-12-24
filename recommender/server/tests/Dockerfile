FROM grihabor/pytest:latest
MAINTAINER Borodin Gregory <grihabor@mail.ru>

RUN pip3 install --no-cache-dir \
        requests \
        flask \
        python-dateutil \
        celery \
        healthcheck

RUN apk update \
 && apk add --virtual .build-deps \
        g++ \
 && pip3 install --no-cache-dir numpy \
 && apk del .build-deps
