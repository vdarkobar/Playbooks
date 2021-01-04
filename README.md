# Ansible
  
<p align="left">
  <a href="https://github.com/vdarkobar/Home_Lab">Home</a>
</p>  
  
Edit Ansible configuration file:
```
sudo nano /etc/ansible/ansible.cfg
```
  
Populate with the required data:
```
sudo nano /etc/ansible/hosts
# or
sudo nano /etc/ansible/inventory
# or
sudo nano Playbooks/inventory
```
```
[all:vars]

# Username for ssh connection
ansible_user=darko

# Run commands as root user?
ansible_become=yes

# How do I become root user? Use sudo.
ansible_become_method=sudo

# Python interpreter version
ansible_python_interpreter='/usr/bin/env python3'

# Password for sudo
#ansible_become_pass='<pass>'

[servers]
<ip1>

# Aliases
server1 ansible_host=<ip2>
server2 ansible_host=<ip3>
```
  
### Clone this git repository:
```
git clone https://github.com/vdarkobar/Playbooks.git
```
