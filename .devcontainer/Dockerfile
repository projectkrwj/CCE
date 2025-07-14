FROM ubuntu:20.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt update && apt install -y \
    python3 python3-pip python3-dev \
    gdb gdb-multiarch git curl wget gcc make \
    libssl-dev libffi-dev build-essential \
    tmux unzip vim net-tools iproute2

RUN pip3 install --upgrade pwntools

RUN curl -fsSL https://gef.blah.cat/sh | bash
