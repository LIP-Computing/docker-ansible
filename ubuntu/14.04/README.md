[![License](http://img.shields.io/:license-apache-blue.svg?style=flat-square)](http://www.apache.org/licenses/LICENSE-2.0.html)

# ansible-ubuntu14.04

Docker image with ansible based on the [official Ubuntu Docker Image](https://registry.hub.docker.com/_/ubuntu/)

## Installed packages

Base:

- [Ubuntu Trusty (14.04) minimal](http://packages.ubuntu.com/trusty/ubuntu-minimal)

Image specific:
- ansible

## Build

```bash
docker build --rm -t ansible-ubuntu14.04 .
```

## Usage

```bash
$ docker run -it ansible-ubuntu14.04 /bin/bash
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
