# Ubuntu desktop

Configure ubuntu desktop via ansible.

```bash
sudo apt update
sudo apt install git ansible
```

Clone this repository and apply the necessary playbooks.

```bash
ansible-playbook ./playbook-user.yml

cp my.inventory.example my.inventory

sudo bash

ansible-playbook -i ./my.inventory ./playbook-common.yml
ansible-playbook -i ./my.inventory ./playbook-samba.yml
ansible-playbook -i ./my.inventory ./playbook-docker.yml
ansible-playbook -i ./my.inventory ./playbook-golang.yml
ansible-playbook -i ./my.inventory ./playbook-vscode.yml
ansible-playbook -i ./my.inventory ./playbook-laptop.yml
ansible-playbook -i ./my.inventory ./playbook-reaper.yml
ansible-playbook -i ./my.inventory ./playbook-virtualbox.yml
```

### Golang source

Install Golang from source.

```
ansible-playbook -i ./my.inventory ./playbook-golang-src.yml
```
