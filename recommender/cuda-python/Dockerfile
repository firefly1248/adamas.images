FROM nvidia/cuda:8.0-cudnn5-runtime-ubuntu16.04
MAINTAINER Borodin Gregory <grihabor@mail.ru>

WORKDIR /root

RUN apt update \
 # install python 3.6
 && apt install -y software-properties-common \
 && add-apt-repository ppa:jonathonf/python-3.6 \
 && apt update \
 && apt install -y \
        wget \
        python3.6 \
        python3.6-dev \
        python3.6-venv \
 # install pip 3.6
 && wget https://bootstrap.pypa.io/get-pip.py \
 && python3.6 get-pip.py \
 && rm -f get-pip.py \
 && apt autoremove \
 # create new links
 && rm -f /usr/local/bin/pip3 \
 && ln -s /usr/local/bin/pip /usr/local/bin/pip3 \
 && rm -f /usr/bin/python3 \
 && ln /usr/bin/python3.6 /usr/bin/python3
