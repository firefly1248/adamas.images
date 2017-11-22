FROM grihabor/cuda:python
MAINTAINER Borodin Gregory <grihabor@mail.ru>

RUN apt update \
 && apt install -y \
        g++ \
        python3-tk

RUN pip3 install --no-cache-dir \
        numpy==1.12 \
        scipy==0.19 \
        h5py==2.7

RUN pip3 install --no-cache-dir \
        scikit-image==0.13 \
        scikit-learn==0.18

RUN pip3 install --no-cache-dir \
        tensorflow-gpu \
        keras

