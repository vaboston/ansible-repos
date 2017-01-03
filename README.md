Ansible Roles:
=============

 This repo contains all the Ansible roles that I've written to my personal infrastructure.

 **Note:** Be very careful to run these roles directly to the Production, please first try them on the Testing Environment before using them to Production.

### Requirements:

We need Ansible software to be installed in order to use these roles, means Roles can be run from any machine that have Ansible installed on.

Here are the steps to install the Ansible on Ubuntu 16.04 LTS:
```bash
sudo apt-add-repository -y ppa:ansible/ansible
sudo apt-get update
sudo apt-get install -y ansible
```
* [Ansible Introduction] - Very good and detail Ansible Introduction 

### To use any Role:

Edit the `hosts` file, enter the server ip/name on which you want to deploy the role(s). Then modify the `site.yml` file, mentioned the role that you want to use and then run this command:
```
ansible-playbook -i hosts playbook.yml
```
**Note:** Please don't forget to change `arbab` with your username
