# Services

## Installation

Update and upgrade apt package repository

```bash
sudo apt update && sudo apt upgrade
```

Install Ansible and Git

```bash
sudo apt install ansible git
```

Clone repository

```bash
git clone https://github.com/spencerdennison/services.git
```

Change into Ansible directory

```bash
cd services/ansible
```

Run Ansible playbooks

```bash
ansible-playbook local.yml --ask-become-pass --ask-vault-pass
```

## Post-Installation

Add device to Tailscale network

```bash
sudo tailscale up
```

Reboot

```bash
sudo reboot
```

