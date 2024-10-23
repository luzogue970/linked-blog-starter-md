Definition

différents type de virtualisation

## Definition

faire fonctionner sur une machine physique plusieurs machines comme si elles fonctionnaient sur une machine simple

- Machine simple : application / [[OS]] / Hardware
- virtualisation = application / [[OS]] / Hardware de la machine Hôte

Hyperviseur :

- contrôle processeur et ressource de la machine hôte
- Alloue à chaque VM les ressources dont elle a besoin
- s’assure que ses VM n’interfèrent pas l’une avec l’autre

2 type d’hyperviseur :

- Bare metal :
    - logiciel qui s’exécute sur le hardware
    - hyperviseur = outil de control de l’os
    - système d’exploitation est exécuté au dessus hardware (modèle le plus répandue en entreprise)
- Host metal :
    - logiciel qui s’exécute à l’intérieur d’un autre système

![[/Untitled 24.png|Untitled 24.png]]

  

## différents type de virtualisation

  

- virtualisation [[Virtualisation]]

Système virtualisé à partir de l’os

- virtualisation de poste travail : os de poste de travail virtualisé
    - VDI : virtual Desktop Infrastructure : poste de travail hébergé dans un data center (comme Teamviewver)
    - streaming d’os : Os démarre a partir d’un disque installé sur le réseau et charge de façon sélectives les app demandé par l’utilisateur à partir d’un serveur distant

![[/Untitled 1 10.png|Untitled 1 10.png]]

- virtualisation d’application
    - virtualisation de sessions : exécuté côté serveur. Ensemble des données app dans datacenter app ⇒ sur navigateur internet ou client installé sur le pc
    - bulle applicative : installation par streaming d’une app sur le poste de travail
        - administrateur met a dispositions des app sur un serveur distant. Utilisateur se connecte au réseau, télécharge les application autorisé sur son poste.
        - quand le client veut utiliser une application, il clique sur l’app et la reçoit la bulle applicative en streaming. et il l’exécute en local