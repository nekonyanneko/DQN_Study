#利用するUbuntuのイメージ
FROM ubuntu:14.04　

MAINTAINER SHUN MORITA

RUN apt-get update
RUN apt-get install -y vim
RUN apt-get install -y wget

# intall python pip
RUN apt-get install -y --no-install-recommends \
 python \
 python-dev \
 python-pip \
 python-numpy \
 python-scipy \
 libffi-dev \
 libssl-dev \
 libhdf5-dev \
 libblas-dev \
 liblapack-dev \
 gfortran \
 && apt-get clean \
 && rm -rf /var/lib/apt/lists/

RUN pip install -U pip
RUN pip install ndg-httpsclient numpy scipy protobuf h5py chainer
