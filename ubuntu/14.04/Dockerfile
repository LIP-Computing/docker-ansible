# docker build -t ansible-ubuntu:14.04 .

FROM ubuntu:14.04

# Install ansible repository
RUN apt-get update -y
RUN apt-get install software-properties-common -y
RUN apt-add-repository ppa:ansible/ansible

RUN apt-get update && \
    apt-get install -y \
        ansible \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

