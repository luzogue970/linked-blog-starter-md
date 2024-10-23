Definitions

message constitué de

Fonctionnement MOM

2 utilisation du MOM

## Definitions

MOM

Message Oriented Middleware

middle d’échange asynchrone

## message constitué de

- données applicative
- entête (caractéristique technique : id , date du message…)
- propriété (diffèrent en fonction de l’application utilisatrice)

  

## Fonctionnement MOM

- application a envoie un message
- MOM utilise une file d’attente / (queu) ⇒ broker message pour stocker le message
- émetteur de destinataire n’ont pas besoin d’être connecté simultanément.
- MOM accuse réception du message 1
- MOM envoie au destinataire quand celui-ci le demande.
- le destinataire accuse la réception

  

## 2 utilisation du MOM

- QUEU message transmit à une application (point à point)
- Topic : message transmit à toute les applications souscriptrice(Observer Pattern)