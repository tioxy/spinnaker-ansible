aws-iam-authenticator
=========

Installs [Golang](https://github.com/golang/go) and [aws-iam-authenticator](https://github.com/kubernetes-sigs/aws-iam-authenticator).
Both are required if you want to run [Spinnaker](https://www.spinnaker.io/) with [EKS](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html) from [AWS](https://aws.amazon.com/).

Requirements
------------

- Ubuntu 16.04

Role Variables
--------------

Stay with the */defaults/main.yml* values.
```yaml
GOLANG_REPO: PPA for latest Golang distribution
GOLANG_PACKAGE: the package to be installed
```

Example Playbook
----------------

```yaml
- hosts: all

  roles:
    - role: aws-iam-authenticator
```

License
-------

MIT

Author Information
------------------

Created by [@tioxy](https://github.com/tioxy)
