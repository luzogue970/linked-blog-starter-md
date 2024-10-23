  

## Def

Permet de modifier des objets dynamiquement

## Cas d’utilisations

  

Au lieu de s’enfermer dans une abstraction sur un objet ou veut couvrir un grand nombre de cas qui ont des points commun ⇒ on va faire un décorateur

  

## Utilisation

une interface avec des méthode liées à l’objet

un objet concret qui implémente cette interface avec des valeurs “de base”

l’abstract décorateur : classe abstraite qui implémente l’interface, prend en paramètre de constructeur un objet du type de l’interface considéré comme partiel.

le décorateur concret qui modifie le partial item pour y ajouter ses particularité

  

  

## Diagramme

![[/Untitled 42.png|Untitled 42.png]]