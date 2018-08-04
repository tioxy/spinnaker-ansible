awscli
=========

Installs [Python 3](https://www.python.org/) and [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-welcome.html).
Both are required if you want to run [Spinnaker](https://www.spinnaker.io/) inside [AWS](https://aws.amazon.com/).

Requirements
------------

- Ubuntu 16.04

Role Variables
--------------

Stay with the */defaults/main.yml* values.
```yaml
PYTHON_PACKAGES: necessary packages to install Python
```

Example Playbook
----------------

```yaml
- hosts: all

  roles:
    - role: awscli
```

License
-------

MIT

Author Information
------------------

Created by [@tioxy](https://github.com/tioxy)
