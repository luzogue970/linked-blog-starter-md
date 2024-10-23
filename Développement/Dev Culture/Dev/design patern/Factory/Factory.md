Def

quand l’utiliser

diagramme:

utilisation concrète

autre

simple factory

Factory Method

Abstract Factory

  

## Def

quand une méthode renvoie une parmi plusieurs class possibles qui découlent d’une super class

  

## quand l’utiliser

- quand on ne sait pas à l’avance l’objet qu’on va créer. (parce que c’est aléatoire ou pas prédictible
- pour utiliser que les class d’une issue de la même super class (avec la même hiérarchie donc)
- >>>>quand on veut éviter à l’utilisateur de devoir connaitre toutes les sub class
- >>>> pour encapsuler la création d’objet

## diagramme:

![[/Untitled 39.png|Untitled 39.png]]

  

## utilisation concrète

au lieu de mettre 12 if dans le main on va les mettre dans la factory

puis on utilise la factory

## autre

### simple factory

not a pattern

### Factory Method

on veut créer un object qui a pour super class x mais on ne sait pas exactement quelle sous classe on veut créer

  

### Abstract Factory