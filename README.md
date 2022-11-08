# Role Ansible pour l'installation de Docker 

Ce rôle install docker sur une machine Ubuntu ou CentOS.

## Prerequis
- Ubuntu ou CentOS.

## How to configure it
- renseigner le user et password dans group_vars/servers 
- renseigner les machines distantes dans hosts.txt

## How to use it ?
Avec SSH keys:
```bash
ansible-playbook playbook_ready_role.yaml
```
Sans SSH keys:
```bash
ansible-playbook playbook_ready_role.yaml -kK
```
kK pour saisir le mot de passe admin

Avec un autre fichier d'inventaire:
```bash
ansible-playbook playbook_ready_role.yaml -i <new_inventory>
```
