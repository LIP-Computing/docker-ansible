# docker build --rm -t ansible-ubuntu14.04 .

FROM ubuntu:14.04
MAINTAINER Mario David <mariojmdavid@gmail.com>
LABEL description="Run ansible roles and playbooks"

RUN apt-get update -y
RUN apt-get install software-properties-common -y
RUN apt-add-repository ppa:ansible/ansible

RUN apt-get update \
    && apt-get install -y ansible wget \
    && apt-get clean \
    && echo "localhost ansible_connection=local" > /etc/ansible/hosts

