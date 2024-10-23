Def

quand l’utiliser

diagramme:

utilisation concrète

bénéfices

négatif

## Def

Un objet appelé **Subject** a une liste de ses dépendants appelé **Observers** et les notifie automatiquement à chaque changement, habituellement en appelant leur méthode

subject > observer = publisher > subscriber

## quand l’utiliser

- quand on a besoin que plusieurs autre objets reçoivent un update lorsque un autre objet change

## diagramme:

![[/Untitled 37.png|Untitled 37.png]]

## utilisation concrète

  

  

## bénéfices

le subject n’a rien besoin de savoir à propos de l’observer

## négatif

le subject peut envoyer des updates qui n’intéressent pas l’observer