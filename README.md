# Spinnaker Ansible

#### - [Purpose](README.md#purpose)
#### - [Requirements](README.md#requirements)
#### - [Installing Requirements](README.md#installing-requirements)
#### - [Getting Started](README.md#getting-started)

## [Purpose](#purpose)
-----
Purpose here

## Provisioned Content
-----
By running this playbook, you will install:
- aws-iam-authenticator
- awscli
- docker
- halyard
- kubectl

## [Requirements](#requirements)
-----
#### Desired host
- Python >= 2.7

#### Your host
- Python >= 2.7
- PIP

## [Installing Requirements](#installing-requirements)
-----
[Click here](README.md#getting-started) if you already have all requirements
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

3. You are up and running to start configuring Spinnaker. Check out **[spinnaker-the-easy-way](https://github.com/tioxy/spinnaker-the-easy-way)** to start using Halyard and configure spinnaker.
