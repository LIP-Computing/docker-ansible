[![License](http://img.shields.io/:license-apache-blue.svg?style=flat-square)](http://www.apache.org/licenses/LICENSE-2.0.html)
[![](https://images.microbadger.com/badges/image/lipcomputing/ansible-ubuntu16.04.svg)](http://microbadger.com/images/lipcomputing/ansible-ubuntu16.04 "Get your own image badge on microbadger.com")

# ansible-ubuntu16.04

Docker image with ansible based on the [official Ubuntu Docker Image](https://registry.hub.docker.com/_/ubuntu/)

## Installed packages

Base:

- [Ubuntu Xenial (16.04) minimal](http://packages.ubuntu.com/xenial/ubuntu-minimal)

Image specific:
- ansible

## Build

```bash
docker build --rm -t ansible-ubuntu16.04 .
```

## Usage

```bash
$ docker run -it ansible-ubuntu16.04 /bin/bash
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
