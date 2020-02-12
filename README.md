# Management d’application cloud
## Pré-requis 
### Configurations
Avoir 2 machines (sous debian 10 dans mon cas)

+ VM1 avec une adresse 192.168.1.50
+ VM2 avec une adresse 192.168.1.95
+ Une connexion à internet
+ Avoir `python` et `python3` d'installé
+ Avoir `python-apt` et `pyton3-apt` d'installé

### SSH
Mettre en place une authentification par clés sans mot de passe afin de faciliter l'execution des commandes Ansible

## Déploiement 

Afin de lancer le déploiement complet de l'infrastructure, on lancera le fichier `playbooks/main.yml`

Pour se faire, taper la commande `ansible-playbook -i hosts playbooks/main.yml -u root`

## Problèmes rencontrés (non-patché)
+ la version 5.8 de npm n'est pas compatible avec la vesrion 10 du nodeJS installé.
+ Quelques APT UPDATE ne passent pas.
