# docker build -t ansible-centos:6 .

FROM centos:6

RUN yum -y update; yum clean all
RUN yum -y install epel-release; yum clean all

RUN yum -y install \
    wget \
    ansible \
    && yum clean all

