============GESTION DES UTILISATEURS AVEC ANSIBLE=============
#  GESTION DES UTILISATEURS AVEC ANSIBLE

##  Description

Ce projet permet d’automatiser la gestion des utilisateurs (ajout, suppression, configuration SSH) sur des serveurs distants grâce à Ansible. Il facilite l’administration système en centralisant les opérations courantes liées aux comptes utilisateurs.

---

## Objectifs

- Automatiser la **création, suppression et mise à jour** des utilisateurs.
- Assurer un **accès SSH sécurisé** avec des clés publiques.
- Faciliter la **maintenance** des utilisateurs via un playbook Ansible réutilisable.

---

## Fonctionnalités

- Ajout automatique de comptes utilisateurs.
- Suppression ou désactivation des comptes existants.
- Déploiement des clés SSH sans mot de passe.
- Support de plusieurs serveurs (webserver, dbserver).
- Gestion simple via des fichiers YAML.

---

## Prérequis

- Ansible installé sur la machine de gestion :
  ```bash
  sudo apt install ansible

 ## Arborescence du Projet
.
├── ansible-users/
│   ├── dbserver_users.yml         # Utilisateurs pour le serveur de base de données
│   ├── webserver_users.yml        # Utilisateurs pour le serveur web
│   ├── manage_users.yml           # Playbook général de gestion des utilisateurs
│   └── inventory                  # Fichier d'inventaire listant les hôtes cibles
├── README.md                      # Documentation du tout le projet


