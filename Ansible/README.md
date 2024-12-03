# Introduction
There are an exapmle for Ansible. 

# How Can I Create ?

- Connect SSH
- Create inventory file:
```bash
touch inventory.yml
```
- Or write hosts on `/etc/ansible/hosts` file:
```ini
[windows]
192.0.2.50
[linux]
192.0.3.50
```
- Test connection to hosts:
```bash
ansible all -m ping
# OR
ansible all -m ping -i inventory.yaml
```
- Create playbook file. It is include jobs for remote server:
```bash
touch nginx.yml
````
- Now, we can run our playbook file:
```bash
ansible-playbook -i inventory.yml nginx.yml
# OR
ansible-playbook nginx.yml
```

It is basically:)

***Note:*** This file is still being worked on. It will include more information about the files.