ARG VARIANT=ubuntu
FROM ${VARIANT}:latest
USER root

RUN export DEBIAN_FRONTEND=noninteractive && apt-get update \
    && apt-get -y upgrade && apt-get -y install --no-install-recommends \
    build-essential cmake gdb \
    && apt-get clean -y && rm -rf /var/lib/apt/lists/*
