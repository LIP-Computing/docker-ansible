# docker build --rm -t ansible-centos7 .

FROM centos:7

RUN yum -y update; yum clean all
RUN yum -y install epel-release; yum clean all

RUN yum -y install \
    wget \
    ansible \
    && yum clean all \
    && echo "localhost ansible_connection=local" > /etc/ansible/hosts

