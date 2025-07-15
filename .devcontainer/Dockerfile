# .devcontainer/Dockerfile

FROM ubuntu:20.04

ENV DEBIAN_FRONTEND=noninteractive
ENV LANG en_US.UTF-8
ENV LC_ALL en_US.UTF-8

# 필수 패키지 설치
RUN apt update && apt install -y \
    software-properties-common \
    curl gdb git python3.11 python3.11-venv python3.11-dev python3.11-distutils \
    locales unzip tmux vim \
 && locale-gen en_US.UTF-8

# pip 설치
RUN curl -sS https://bootstrap.pypa.io/get-pip.py | python3.11

# python3 기본 링크 변경
RUN ln -sf /usr/bin/python3.11 /usr/bin/python3

# pwndbg 설치
RUN git clone https://github.com/pwndbg/pwndbg ~/pwndbg \
 && cd ~/pwndbg \
 && git checkout 2024.08.29 \
 && ./setup.sh

# 시작 시 위치 설정
WORKDIR /workspaces/CCE
