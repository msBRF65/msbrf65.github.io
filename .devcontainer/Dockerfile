ARG BASE_IMAGE=klakegg/hugo:0.101.0-ubuntu
FROM ${BASE_IMAGE}

ARG WORK_DIR=/src
ARG USER_NAME=ubuntu

RUN apt-get update && \
    apt-get install -y git

RUN useradd -ms /bin/sh ${USER_NAME}
USER ${USER_NAME}

WORKDIR /src