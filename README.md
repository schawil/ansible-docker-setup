# Ansible Docker Installation

Ce projet contient un playbook Ansible pour automatiser l'installation de Docker sur une VM Debian 11 installée avec Vagrant.

## Structure du projet

- `inventory.ini` : Fichier d'inventaire pour spécifier les hôtes distants.
- `playbook.yml` : Playbook principal pour appeler le rôle Docker.
- `roles/docker/tasks/main.yml` : Tâches Ansible pour installer Docker.

## Instructions

1. Clonez ce dépôt sur votre machine locale :

   git clone https://github.com/schawil/ansible-docker-setup.git
   cd ansible-docker-setup

2.  Assurez-vous que votre machine cible est accessible via SSH et définissez les informations nécessaires dans inventory.ini
 
3. Lancez le playbook Ansible:
   ```bash
	 ansible-playbook -i inventory.ini playbook.yml



