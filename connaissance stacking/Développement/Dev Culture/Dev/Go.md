### général

go :

- langage compilé
    - code source transformé par un compilateur avant d’être lancé. la code transformé en binaire est directement lisible par la machine
        - permet d’optimiser les performances lors de l'exécution.
- typage statique
- Conçu pour la simplicité et l'efficacité
- Support natif pour la concurrence (Goroutines)
- Gestion automatique de la mémoire (Garbage Collection)
- Système de paquetage (modules)
- Forte communauté et écosystème
- Créé par Google
- version actuelle : 1.22.4

### Go module

- permet de gérer les dépendances de manière plus efficace et reproductible
- go.mod : contient nom du module / dépendances
- go.sum : enregistre les hachages cryptographiques des versions spécifiques des modules utilisés dans votre projet.

### Goroutine

- permet de gérer du mutlithread avec go fct …
- Channel permet de gérer la transmition de donné entre les thread
- pour éviter les deadLock ⇒ select / buffer

## gin

- framework golang

### Gorm

orm utilisable avec gin

### pas de classes mais des struct

- qui ont de la composition ⇒ embeded
- method promu avec l’item embeded