# Ansible
  
Edit Ansible configuration file:
```
sudo nano /etc/ansible/ansible.cfg
```
  
Populate Ansible hosts file with the required data:
```
sudo nano /etc/ansible/hosts
```
```
[all:vars]                                                  # Change: <user>, <bastion pass>, ip
# Username for ssh connection
ansible_user=<user>
# Run commands as root user?
ansible_become=yes
# How do I become root user? Use sudo.
ansible_become_method=sudo
# Python interpreter version
ansible_python_interpreter='/usr/bin/env python3'
# Password for sudo
ansible_become_pass='<bastion pass>'

#

[servers]
ip
ip
```
