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

sudo ansible-playbook -i ./my.inventory ./playbook-common.yml
sudo ansible-playbook -i ./my.inventory ./playbook-ufw.yml
sudo ansible-playbook -i ./my.inventory ./playbook-samba.yml
sudo ansible-playbook -i ./my.inventory ./playbook-docker.yml
sudo ansible-playbook -i ./my.inventory ./playbook-golang.yml
sudo ansible-playbook -i ./my.inventory ./playbook-vscode.yml
sudo ansible-playbook -i ./my.inventory ./playbook-laptop.yml
sudo ansible-playbook -i ./my.inventory ./playbook-virtualbox.yml
sudo ansible-playbook -i ./my.inventory ./playbook-php8.2.yml
sudo ansible-playbook -i ./my.inventory ./playbook-sampler.yml
sudo ansible-playbook -i ./my.inventory ./playbook-yandex-disk.yml
```

### Golang from source

```bash

sudo ansible-playbook -i ./my.inventory ./playbook-golang-src.yml
```

### Sound pipeware

```bash
sudo ansible-playbook -i ./my.inventory ./playbook-sound-pipewire.yml

systemctl --user restart pipewire.service pipewire-pulse.socket
```

### Soundrecord

```bash

sudo ansible-playbook -i ./my.inventory ./playbook-soundrecord-reaper.yml
sudo ansible-playbook -i ./my.inventory ./playbook-soundrecord-vst.yml
sudo ansible-playbook -i ./my.inventory ./playbook-soundrecord-realtime.yml
```
