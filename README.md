Ansible role: Terraform
=========

This role helps you to install pip3 on your linux machine.


|Travis|GitHubActions|Quality|Downloads|Version|
|------|-------------|-------|---------|-------|
|[![travis](https://travis-ci.com/amine7777/ansible-role-pip3.svg?branch=master)](https://travis-ci.com/amine7777/ansible-role-pip3)|[![github](https://github.com/amine7777/ansible-role-pip3/workflows/CI/badge.svg)](https://github.com/amine7777/ansible-role-pip3/actions)|[![quality](https://img.shields.io/ansible/quality/50498)](https://galaxy.ansible.com/amine7777/pip3)|[![downloads](https://img.shields.io/ansible/role/d/50348)](https://galaxy.ansible.com/amine7777/pip3)|[![Version](https://img.shields.io/github/release/amine7777/ansible-role-pip3.svg)](https://github.com/amine7777/ansible-role-pip3/releases/)|

![](pip3.jpg)

Requirements
------------
- Linux machine
- Ansible 2.9

Role Variables
--------------
These variables helps to manage pip3 installation.

You can specify your pip3 version in this variable.
```yaml
pip3_version: 0.13.1
pip3_arch: amd64
pip3_directory_path: /usr/local/bin
```
This is the url where pip3 will be downloaded.
```yaml
pip3_download_url: 'https://releases.hashicorp.com/pip3/{{ pip3_version }}/pip3_{{ pip3_version }}_linux_{{ pip3_arch }}.zip'
```
This is the path where packer binary will be stored.
```yaml
pip3_directory_path: /usr/local/bin
```

Example Playbook
----------------

```yaml
- hosts: all
  roles:
     - amine7777.pip3
```


Author Information
------------------

- [Amine Kahlaoui](https://github.com/amine7777), DevOps engineer.
