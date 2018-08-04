halyard
=========

Installs [Halyard](https://www.spinnaker.io/setup/install/halyard/#install-on-debianubuntu-and-macos).
Required by [obivous reasons](https://www.spinnaker.io/setup/install/).

Requirements
------------

- Ubuntu 16.04

Role Variables
--------------

Stay with the */defaults/main.yml* values.
```yaml
HALYARD_INSTALLATION_SCRIPT: link to download halyard installation script
```

Example Playbook
----------------

```yaml
- hosts: all

  roles:
    - role: halyard
```

License
-------

MIT

Author Information
------------------

Created by [@tioxy](https://github.com/tioxy)
