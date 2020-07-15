# Ansible Playground

### Step 1
Run containers with docker-compose:
```bash
cd ansible-playground
docker-compose up -d
```
Check containers
```bash
docker ps
```
### Step 2
Connect to container with ansible:
```bash
ssh root@172.30.1.1
```
password: toor

### Step 3
Ping hosts:
```bash
cd /etc/ansible
ansible all -m ping
```
You can find ansible hosts config and playbooks in control_node/ansible, .ssh/known_hosts in control_node/ssh

### Step 4
Run playbooks:
```bash
cd /etc/ansible/playbooks
ansible-playbook install_nginx.yml 
```

Available playbooks:
- install_nginx.yml
- uninstall_nhinx.yml
