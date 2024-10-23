[[Cloud]]

IAAS

CAAS

PAAS

FAAS

SAAS

## IAAS

- [ ] tester : **Amazon Web Services (AWS), Microsoft Azure, Google Cloud, DigitalOcean et Linode**.

Infrastructure as a service (partie infrastructure du cloud)

- Fournit des instance [[OS]] / ensemble infrastructure sous-jacente ⇒ serveur / stockage / réseau
- client gère Os / midlewear et apllicatif

  

  

## CAAS

conteneur as a service

- [ ] tester : Les fournisseurs de cloud public tels que Google, Amazon Web Services (AWS), Microsoft ou IBM ont tous une offre CaaS à leur catalogue / **AWS propose Amazon EC2 Container Service (ECS)**

entre IAAS et PAAS

- permet au client de déployer et gérer des [[Docker]] pendant tout leur cycle de vie

différence entre PAAS et CAAS :

CAAS n’inclut pas d’outil de dev et donc l’app doit être dev séparément

## PAAS

- [ ] tester : **AWS Elastic Talk et Google App Engine**

Plateform as a service :

- Offre framework / compilateur
- Propose serveur web / système de gestion de BDD

Permet au client de se focaliser sur le développement applicatif

C’est la solution faite pour les dev (mathieu)

  

## FAAS

- [ ] **AWS Lambda d'Amazon**. **Google Cloud Functions**

Function as a service (serverless)

voir vidéo

entre PAAS et SAAS

- sert pour les taches planifier (date ou fréquence) / workflow planifier
- dev responsabilité de coder ses fonctions

objectif PAAS simplifier dev application, quand une app est déployée sur PAAS l’appli tourne en continue sur le serveur

FAAS possibilité de déclencher une seule fonction quand on en a besoin donc fonction ne ne tournent pas tant qu’elles ne sont pas sollicité

## SAAS

Software as a service

- fournit application prête a l’emploie
- accessible via le navigateur
- client n’a pas a gérer mise a jour et infrastructure sous-jacente
- exemple google doc / office 365