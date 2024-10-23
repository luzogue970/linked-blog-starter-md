Definition

règle des filtrage

Type de fireWall

DMZ

## Definition

sécuriser un réseau en définissant les communication autorisées ou interdites

contrôle flux entrant sortant et accepte ou rejette des communications

permet de connecter 2 réseaux

réseau interne d’une entreprise : confiance forte

internet : confiance faible

  

## règle des filtrage

- origine / destination des packets
- les données
- options dans les données (fragmentation / validité)
- les utilisateurs

  

## Type de fireWall

- Stateless packet inspection (par feu sans état)
    - regarde chaque packet et le compare a une liste de règle de filtrage ACL(access control list)
    - regarde ip source / destination /// port source / destination
- statefull packet inspection
    - vérifie que chaque packet d’une connexion est bien la suite du précédant packet et la réponse à un packet dans l’autre sens
- firewall applicatif
    - niveau 7 de OSI
    - filtré par processus dédié : http filtré par http …
    - joue le rôle de proxy applicatif (voir proxy
- parfeu identifiant
    - filtrage par utilisateur et pas par adresse ip / mac
- firewall personnel
    - contrôle l’accès de l’ordinateur sur lequel il est installé
    - permet de repérer et d’empêcher l’ouverture d’app non connecté

## DMZ

demilitarized zone

pour les machines pouvant accéder à internet