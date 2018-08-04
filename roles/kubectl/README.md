kubectl
=========

Installs [kubectl](https://github.com/kubernetes/kubectl).
Required if you want to support [Kubernetes](https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/) for your [Spinnaker](https://www.spinnaker.io/) installation.

Requirements
------------

- Ubuntu 16.04

Role Variables
--------------

Stay with the */defaults/main.yml* values.
```yaml
GOOGLE_GPG_KEY: google gpg key
KUBECTL_REPO: kubernetes deb packages repository
```

Example Playbook
----------------

```yaml
- hosts: all

  roles:
    - role: kubectl
```

License
-------

MIT

Author Information
------------------

Created by [@tioxy](https://github.com/tioxy)
