# Spinnaker Ansible

#### - [Purpose](README.md#purpose)
#### - [What does it install?]()
#### - [Requirements](README.md#requirements)
#### - [Getting Started](README.md#getting-started)

</br>

## [Purpose](#purpose)
-----

It was made to install Halyard and some tools which are necessary to make Spinnaker and AWS to work properly. This version only supports Halyard installation, but Spinnaker Configuration and Deployment will be added in the future.

By running this playbook, you will install:
- [aws-iam-authenticator](roles//README.md)
- [awscli](roles/awscli/README.md)
- [docker](roles/docker/README.md)
- [halyard](roles/halyard/README.md)
- [kubectl](roles/kubectl/README.md)

</br>

## [Requirements](#requirements)
[Click here](README.md#getting-started) if you already have all requirements

-----
#### Desired host
- Ubuntu == 16.04
- Python >= 2.7

#### Your host
- Python >= 2.7
- PIP

</br>

#### Installing Requirements

1. Install Python and PIP

```sh
# Debian/Ubuntu
sudo apt-get install python python-pip

# CentOS/RHEL
sudo yum install yum-utils epel-release
sudo yum-config-manager --enable epel
sudo yum install python python-pip
```

2. Install Ansible using the PIP distribution

```sh
sudo -i pip install --upgrade ansible
```

</br>

## [Getting Started](#getting-started)
-----
1. Clone the repository
```sh
git clone https://github.com/tioxy/spinnaker-ansible.git
```

2. Edit the *sample-inventory* file and configure the desired host connection following [Ansible Docs](https://docs.ansible.com/ansible/latest/user_guide/intro_inventory.html)

3. Run the file *main.yml*
```sh
ansible-playbook -i sample-inventory master.yml
```

3. You are able to start configuring Spinnaker now. Check out **[spinnaker-the-easy-way](https://github.com/tioxy/spinnaker-the-easy-way)** to start using Halyard and configure spinnaker.
