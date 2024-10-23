Definition

Definition conteneur :

definition docker

Image docker

But

## Definition

### Definition conteneur :

[[Virtualisation]] par conteneur se base sur :

Linux LXC = Linux Containers

- Cloisonnement au niveau de l’os ⇒ faire tourner des environnement linux isolé les uns des autres dans des conteneur partageant le même noyau
- Conteur l’environnement d’exécution comme le processeur, la mémoire vive ou le système de fichier et ne virtualise pas la machine. diff entre VM et Conteneur

**repose sur 2 fonctionnalité de linux :**

- Cgroups / control groups : Permet d’isoler l’utilisation des ressources
- NameSpace : cloisonnement espace de nommage :empêche qu’un groupe puisse voir les espace d’un autre groupe

**Couche intermédiaire du controller :**

- gère les intéraction avec l’OS
- sécurité avec gestion privilège et ressource
- scalabilité dupplication / suppression conteneur
- accessibilité des conteneur à traver API et CLI

### definition docker

docker permet de créer des conteneurs qui vont uniquement contenir des applications avec leur dépendances.

**Docker engine:** fait tourner les docker et sert de controller

![[/Untitled 25.png|Untitled 25.png]]

## Image docker

- Template prêt à l’emploie avec des instructions pour la création de conteneur
- construite a partir d’un Dockerfile / image existante / récupéré sur un registre docker
    - Dockerfile permet de créer une image étape par étape de manière automatisé

![[/Untitled 1 11.png|Untitled 1 11.png]]

## But

docker permet de faciliter et rendre plus rapide le déploiement

facilite le travail des admin système (voir c quoi)