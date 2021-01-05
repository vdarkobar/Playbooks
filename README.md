# Ansible 
## Install Ansible on your Bastion Server
  
<p align="left">
  <a href="https://github.com/vdarkobar/Home_Cloud#proxmox">Home</a>
</p>  
  
### Install Ansible:
```
sudo apt install ansible -y
ansible --version
```
	
### To Install latest version:
```
echo "deb http://ppa.launchpad.net/ansible/ansible/ubuntu bionic main" | sudo tee -a /etc/apt/sources.list
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 93C4A3FD7BB9C367
sudo apt update
sudo apt install ansible -y
sudo ansible --version
```
  
Edit Ansible configuration file:
```
sudo nano /etc/ansible/ansible.cfg
```
    
### Clone this git repository:
```
git clone https://github.com/vdarkobar/Playbooks.git
```
  
Populate with the required data:
```
sudo nano Playbooks/inventory			

# Additional ways to create inventory: sudo nano /etc/ansible/hosts, sudo nano /etc/ansible/inventory
```  
  
Run Playbook:
```
ansible-playbook -i inventory update.yml
```
