docker
=========

Installs [Docker](https://www.docker.com/what-docker).
Required if you want to run [Halyard containerized](https://www.spinnaker.io/setup/install/halyard/#install-halyard-on-docker).

Requirements
------------

- Ubuntu 16.04

Role Variables
--------------

Stay with the */defaults/main.yml* values.
```yaml
DOCKER_GPG_KEY: docker gpg key
DOCKER_REPO: docker deb package repository
DOCKER_REQUIREMENTS: list of requirements to install Docker
```

Example Playbook
----------------

```yaml
- hosts: all

  roles:
    - role: docker
```

License
-------

MIT

Author Information
------------------

Created by [@tioxy](https://github.com/tioxy)
