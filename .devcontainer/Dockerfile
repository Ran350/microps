FROM ubuntu:22.04

RUN apt-get update && apt-get install -y \
    build-essential \
    git \
    iproute2 \
    iputils-ping \
    netcat-openbsd

RUN mkdir -p /dev/net && \
    mknod /dev/net/tun c 10 200 && \
    chmod 0666 /dev/net/tun

CMD ["/bin/bash"]