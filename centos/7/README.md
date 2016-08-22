# ansible-centos7
[![License](http://img.shields.io/:license-apache-blue.svg?style=flat-square)](http://www.apache.org/licenses/LICENSE-2.0.html)

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

## Author

Mario David: LIP Lisbon and Indigo DataCloud

## License

Apache2

