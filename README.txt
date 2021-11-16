# Ubuntu desktop

Configure ubuntu desktop via ansible.

```bash
sudo apt update
sudo apt install git ansible
```

Clone this repository.

```
sudo bash
ansible-playbook ./playbook.yml
ansible-playbook ./playbook-samba.yml
ansible-playbook ./playbook-docker.yml
ansible-playbook ./playbook-vscode.yml
ansible-playbook ./playbook-laptop.yml
```
