> [!important]  
> Conseil de Notion : Utilisez cette page pour garder une trace de vos notes et des passages intéressants. Vous pouvez également faire référence à d’autres pages Notion en tapant la commande [[. Pour en savoir plus, cliquez ici.  

[![](https://www.notion.so)](https://www.notion.so)

**Table des matières**

Def:

creational patern

Factory Method

Abstract Factory

Singleton

Structural Patterns

Adapter

Bridge

Behavior patern

observer

Strategy

Command

Iterator

  

  

[https://refactoring.guru/](https://refactoring.guru/)

créer git pour design patern

  

# Def:

  

  

## creational patern

### Factory Method

[[Factory]]

[[Factory]]

objectif:définit une interface pour créer des objets dans une classe mère, mais délègue le choix des types d’objets à créer aux sous-classes.

Au lieu de devoir changer le code si un nouveau product b doit être géré, le code ne changent pas car product a , b ,c… découlent de product et que le code est couplé a product

(méthode product commune)

éviter que le code soit couplé à une seul classe mais à la classe mère

- interface button découle sur plusieurs buttons(windows / HTML)
- méthode fabrique vide : type de retour ⇒ Button
- deux classes extend la fabrique et sont les fabriques des classes implémentant Button

![[/Untitled 23.png|Untitled 23.png]]

- [x] tester

### **Abstract Factory**

factory avec un niveau de plus au lieu de product : product / service

**en utilisant la fabrique WinFactory tous objets créés de cette fabrique seront obligatoirement du type Windows**

donc dans le cas ci-dessous : 👇

- creation de interfaces button/checkbox⇒ sous-classes implémentent
- création d’une fabrique abstraite qui renvoie interface button / checkbox
- création des concretes fabriques correspondantes aux sous-classes

![[/Untitled 1 9.png|Untitled 1 9.png]]

- [x] tester

### **Singleton**

[[Singleton]]

garantit que l’instance d’une classe n’existe qu’en un seul exemplaire, tout en fournissant un point d’accès global à cette instance

étapes:

- Rendre le constructeur par défaut privé afin d’**empêcher les autres objets d’utiliser l’opérateur** `**new**` **avec la classe du singleton.**
- méthode de création statique qui se comporte comme un constructeur.
    - En coulisse, cette méthode appelle le constructeur privé pour créer un objet et le sauvegarde dans un attribut statique.
    - Tous les appels ultérieurs à cette méthode retournent l’objet en cache.

![[/Untitled 2 8.png|Untitled 2 8.png]]

- [x] tester

## Structural Patterns

### **Adapter**

objectif : type de donnée invalide pour utiliser une librarie. Solution : adapter patern traduis le données en une donnée utilisable par la librairie (exemple XML to JSON)

- service ne pouvant prendre que des données de type Y
- classe adapter convertit données x en données Y

→ mon BoondConnector = grand adaptateur

→ à une plus petit échelle : mapstruct / mapping d’un type de donnée à un autre

- [x] tester

### Bridge

## Behavior patern

### observer

Objectif:certains objets x veulent être alerté de changements sur un objet y (changement peuvent être de type abcd). Au lieu de bombarder les objets x d’info qui peuvent ne pas les intéresser ou que les objets x aillent constamment voir si il y n’a pas de changement.

les objets s’abonnent au changement de y qui les intéressent. et à chaque changement un publisher notify les intéressés

- publisher envoie évènements à d’autre objets possède (sub/unsub/notify)
- les évènement régaissent à la notification si elle les intéresse par un update

exemple gestion event BoondConnector(pas sûr)

![[/Untitled 3 4.png|Untitled 3 4.png]]

  

- [x] tester

### Strategy

Objectif : exécuter différentes stratégies similaires sans toutes les appeler (elles ne sont pas forcément toutes utilisées)

- interface stratégie commune à toutes les strat
- contexte prend en paramètre une Stratégie
- seul le contexte est appelé dans le “main” et exécute stratégies

![[/Untitled 4 3.png|Untitled 4 3.png]]

- [x] tester

### Command

objectif: pour ne pas reproduire le même code 15 fois avec par exemple un code copier pour le bouton copier, un code pour le raccourcis ctrl+C on définit une commande avant de définir un bouton ou un raccourcis puis on assigne cette aux commande aux 2 éléments.

- inteface commandes avec toutes les commandes qui en découlent
- les objet avec lesquelles le user intéragit (shortcut/button)se voient assigner une commande

![[/Untitled 5 3.png|Untitled 5 3.png]]

- [x] tester

### Iterator

- a

  

![[/Untitled 6 3.png|Untitled 6 3.png]]

- [x] tester

[[Observer]]

[[Strategie]]

[[Abstract factory]]

[[Factory]]

[[Builder]]

[[Prototype]]

[[Decorator]]