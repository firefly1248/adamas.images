FROM python:3.6-alpine
MAINTAINER Borodin Gregory <grihabor@mail.ru>

RUN pip3 install --no-cache-dir \
        requests \
        flask \
        python-dateutil \
        celery \
        healthcheck \
        woger

RUN apk update \
 && apk add --virtual .build-deps \
        g++ \
 && pip3 install --no-cache-dir numpy \
 && apk del .build-deps
