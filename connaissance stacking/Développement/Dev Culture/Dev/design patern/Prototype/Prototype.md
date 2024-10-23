  

## def

besoin : créer un nouvel objet qui est une copie d’un autre

  

## Diagram

cas normale : client to prototype sans factory

![[/Untitled 41.png|Untitled 41.png]]

  

Abstract classe extend Clonable ou possède un méthode Clone

PrototypeFactory qui prend un en paramètre de constructeur l’Abstract classe et qui prend une méthode getClone qui renvoie une copie de l’objet.