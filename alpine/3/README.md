[![License](http://img.shields.io/:license-apache-blue.svg?style=flat-square)](http://www.apache.org/licenses/LICENSE-2.0.html)
[![](https://images.microbadger.com/badges/image/lipcomputing/ansible-alpine3.svg)](http://microbadger.com/images/lipcomputing/ansible-alpine3 "Get your own image badge on microbadger.com")

# ansible-alpine3

Docker image with ansible based on the alpine

## Installed packages

Base:

- [1science Alpine 3.4](https://hub.docker.com/r/1science/alpine/)

Image specific:
- ansible

## Build

```bash
docker build --rm -t ansible-alpine3 .
```

## Usage

```bash
$ docker run -it ansible-alpine3 /bin/bash
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
