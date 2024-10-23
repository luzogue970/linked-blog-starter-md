Definition

[https://www.youtube.com/watch?v=msB9AvJ4bTM](https://www.youtube.com/watch?v=msB9AvJ4bTM)

## Definition

Hypertext Transform Protocol

définit les règles de communication pour les échanges sur le web

il est stateless = pas d’historique.

peut être résolue grâce aux cookie / JWT (json web token)

![[/Untitled 31.png|Untitled 31.png]]

HTTPS : utilise chiffrement SSL et TLS pour sécuriser les communication entre le client et le serveur

  

chiffrement SSL / TLS

[https://www.youtube.com/watch?v=7W7WPMX7arI](https://www.youtube.com/watch?v=7W7WPMX7arI)

SSL = Secure Sockets Layer

TLS = transport Layer Security

SSL obsolète

échange normale :

1. p1 envoie sa clé publique à p2
2. p2 chiffre son message avec la clé publique et l’envoie à p1
3. p1 lie le message grâce à sa clé privé lié a sa clé publique qui a chiffré le message
4. puis même chose sens inverse

man in the middle :

il peut lire les conversations de p1 et p2

1. p1 envoie sa clé publique a p2 mais MITM l’intercepte, garde la clé de p1 et renvoie sa propre clé publique a p2
2. p2 crypte le message avec la clé publique de MITM en pesant que c’est celle de p1 puis renvoie à p1
3. MITM intercepte le message qu’il décrypte avec sa clé privé
4. il le chiffre avec la clé publique de p1 et renvoie a p1 qui le déchiffre avec sa clé privé
5. et inversement