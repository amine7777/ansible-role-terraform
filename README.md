# Install Terraform [![amine7777](https://circleci.com/gh/amine7777/install_terraform.svg?style=svg)](https://circleci.com/gh/amine7777/install_terraform)
-------------------------------------------------------------------------------------------
![](terrafom.jpg)

This playbook is an easy way to install Terraform with just adding the last version.

You need to have a Linux OS.
You need to have Ansible already installed.

Please copy and paste these commands

```bash
git clone https://github.com/amine7777/install_terraform
cd install_terraform
ansible-playbook deploy_terraform.yaml -e "terraform_version=0.12.23"
```
