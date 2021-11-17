# Ubuntu desktop

Configure ubuntu desktop via ansible.

```bash
sudo apt update
sudo apt install git ansible
```

Clone this repository.

```bash
ansible-playbook ./playbook-user.yml

cp my.inventory.example my.inventory

sudo bash
ansible-playbook -i ./my.inventory ./playbook-common.yml
ansible-playbook -i ./my.inventory ./playbook-samba.yml
ansible-playbook -i ./my.inventory ./playbook-docker.yml
ansible-playbook -i ./my.inventory ./playbook-vscode.yml
ansible-playbook -i ./my.inventory ./playbook-laptop.yml
```
