  

  

## objectif :

créer un objet de plusieurs autres objets

pourquoi l’utiliser :

- création des parties de l’objet indépendantes de l’objet principale
- cacher la création des parties de l’objet au client pour qu’ils ne dépendent pas l’un de l’autre ?
- seul le builder sait ce qu’il fait ?

  

## diagramme

![[/Untitled 40.png|Untitled 40.png]]

## utilisation

On définit d’abord une **interface** qui possède les setter de l’item que l’on veut créer. On crée **l’objet** et on lui fais implémenter le builder.

On crée ensuite un builder, une interface qui possède les méthode de création des parties de notre objet ⇒ ce builder est implémenté par un builder concert qui possède l’objet dans son constructeur et qui crée toutes les parties de l’objet et les set dans l’objet

  

on a ensuite un ingénieur qui prend en paramètre de constructeur un builder. et qui utilise ce builder pour créer l’objet x et le le renvoyer

  

exemple :

interface robotPart ⇒ implémenté par robot

interface builderRobot ⇒ implémenté par OldRobotBuilder

Ingénieur/directeur utilise un objet de type buildRobot et a deux méthode : createRobot / getRobot

Main : on crée notre builder de type OldRobotBuilder

on crée notre ingénieur qui utilise notre builder et on crée et get le robot