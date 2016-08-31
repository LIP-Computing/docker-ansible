[![License](http://img.shields.io/:license-apache-blue.svg?style=flat-square)](http://www.apache.org/licenses/LICENSE-2.0.html)
[![](https://images.microbadger.com/badges/image/lipcomputing/ansible-centos7.svg)](http://microbadger.com/images/lipcomputing/ansible-centos7 "Get your own image badge on microbadger.com")

# ansible-centos7

Docker image with ansible based on the [official CentOS Docker Image](https://registry.hub.docker.com/_/centos/)

## Installed packages

Base:

- [CentOS (7) minimal](https://hub.docker.com/_/centos/)

Image specific:
- ansible

## Build

```bash
docker build --rm -t ansible-centos7 .
```

## Usage

```bash
$ docker run -it ansible-centos7 /bin/bash
```

The /etc/ansible/hosts is prepared to run the ansible-playbooks on the localhost
with ansible_connection=local

```bash
# ansible-galaxy install <Some role>
# ansible-playbook <Some playbook>
```

License
-------

Apache v2

Author Information
------------------

Mario David: <mariojmdavid@gmail.com>

LIP Lisbon: http://www.lip.pt

Indigo DataCloud: https://www.indigo-datacloud.eu/

