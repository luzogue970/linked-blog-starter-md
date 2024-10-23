Definition

couches

application

Présentation

Session

Transport

Réseau

Liaison

Physique

communication entre deux machines :

utilisation OSI

[https://www.youtube.com/watch?v=msB9AvJ4bTM](https://www.youtube.com/watch?v=msB9AvJ4bTM)

## Definition

Modèle osi ⇒ Open System Interconnection

définit standards des communication entre les machines du réseau

  

  

# couches

## application

- **interface entre l’homme et la machine** ⇒ moteur de recherche, logiciel de messagerie
- protocle SMTP / [[HTTP]] / HTP

![[/Untitled 30.png|Untitled 30.png]]

## Présentation

- **met en forme les données** ⇒ convertir, reformer, compresser
- permet la communication entre des machines travaillant avec différentes représentations de données

## Session

**gère l’organisation des échanges en permettant l’ouverture et la fermeture des sessions entre les machines**

- ouvre des sessions d’échange pour que les machines puissent communiquer
- et interromps la session lorsque l’échange est terminé

## Transport

- **choisis en fonction des contraintes de communication la meilleur manière d’envoyer l’information** : 2 protocoles :
    - UDP : envoie d’info sans garantie de reception ⇒ simple et rapide : flux vidéo / temps réel app
    - TCP : fiables les communication ( accusé de reception ) ⇒ utilisé la ou la livraison de paquet est obligatoire

## Réseau

- **assure le routage des packets entre les noeuds du réseau** d’un point à a b
- protocole IP : gestion de l’adressage IP

## Liaison

- **définit la transmission des données entre 2 machines du même réseau**
- liaison des données grâce aux adresse mac (Medium Access Control)
- protocole : Ethernet, PPP point to point protocole (opérateur)

## Physique

- connexion physique sur le réseau pour l’émission et la réception de bit
- caractéristique physiques de la communication : cables, lien par fibre optiques, wifi / blutooth

  

## communication entre deux machines :

- Modèle théorique :

![[/Untitled 1 14.png|Untitled 1 14.png]]

- Réalité
- Pour communiquer des entêtes sont ajouter pour spécifier le protocole utilisé a chaque niveau de la communication : et les entêtes sont lues et supprimé pendant la lecture de manière symétrique

![[/Untitled 2 11.png|Untitled 2 11.png]]

Modèle TCP/IP :

![[/Untitled 3 6.png|Untitled 3 6.png]]

  

## utilisation OSI

- les équipements réseau n’utilisent qu’une partie du modèle osi

![[/Untitled 4 4.png|Untitled 4 4.png]]