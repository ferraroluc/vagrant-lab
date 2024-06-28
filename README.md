# Vagrant LAB

Build a Vagrant laboratory for testing purposes, mainly for Ansible.

## Requirements

This lab is made for Linux and requires a public-private key pair to connect via SSH to the created machines.

```bash
mkdir ~/.ssh
cd ~/.ssh
ssh-keygen
```

In order to work on Windows, the Vagrantfiles would require some modifications.

## Start

```bash
chmod +x start.sh
./start.sh
```

## Test Ansible

```bash
ansible vagrant -i inventory.ini -m ping
```

## Stop

```bash
chmod +x stop.sh
./stop.sh
```

## Destroy

```bash
chmod +x destroy.sh
./destroy.sh
```

## ToDo

- Adapt fow Windows
- Change CentOS for another supported distribution
