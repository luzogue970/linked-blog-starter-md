  

opérateurs

mergeMap

ConcatMap

ExhaustMap

SwitchMap

observable chaud / froid

froid

chaud

## opérateurs

un train rouge met 5 s pour arriver et un train rouge 6 sec

### mergeMap

MergeMap assure le parallélisme

a chaque fois que la lumière s’allume en x le train x est appelé :

dès que l’observable parent émet l’observable enfant est souscrit

![[/Untitled 20.png|Untitled 20.png]]

### ConcatMap

assure le mise en série des observable enfants

dès que train précédant arrive le train suivant est appelé

![[/Untitled 1 8.png|Untitled 1 8.png]]

### ExhaustMap

tant qu’il y existe un observable enfant en en vie, toutes les émissions de l’observable parent sont ignorées.

![[/Untitled 2 7.png|Untitled 2 7.png]]

### SwitchMap

a chaque fois que la lumière a changer de couleur on a annulé le train précédent( on a annulé la souscription a l’observable enfant précédant)

![[/Untitled 3 3.png|Untitled 3 3.png]]

  

## observable chaud / froid

### froid

observables froids **produisent des valeurs indépendamment de l'existence de souscriptions.**

observables froids **recommencent à produire des valeurs** à partir du début pour chaque nouvelle souscription.

image : observables froids sont comme des enregistrements vidéo que vous pouvez rejouer à volonté.

### chaud

observables chauds ne **produisent des valeurs que lorsqu'il y a des souscriptions actives.**

observables chauds **continuent à produire des valeurs** à partir du moment où la première souscription est active.

image : observables chauds sont comme une retransmission en direct d'un événement qui se produit en temps réel.

  

  

mathieuleprovost@macbook-pro-de-mathieu customer-web-gateway % ng update  
Using package manager: npm  
Collecting installed dependencies...  
Found 47 dependencies.  
We analyzed your package.json, there are some packages to update:  

```Plain
  Name                                    Version                  Command to update
 -------------------------------------------------------------------------------------
  @angular-eslint/schematics              15.2.1 -> 17.3.0         ng update @angular-eslint/schematics
  @angular/cdk                            15.2.9 -> 16.2.9         ng update @angular/cdk@16
  @angular/cli                            15.2.9 -> 16.2.9         ng update @angular/cli@16
  @angular/core                           15.2.9 -> 16.2.9         ng update @angular/core@16

There might be additional packages which don't provide 'ng update' capabilities that are outdated.
You can update the additional packages by running the update command of your package manager.
```

  

npm ERR! code ERESOLVE  
npm ERR! ERESOLVE could not resolve  
npm ERR!  
npm ERR! While resolving: @nebular/auth@11.0.0  
npm ERR! Found: @angular/common@17.3.0  
npm ERR! node_modules/@angular/common  
npm ERR! @angular/common@"^17.3.0" from the root project  
npm ERR! peer @angular/common@"^16.0.0 || ^17.0.0" from @angular/cdk@16.2.14  
npm ERR! node_modules/@angular/cdk  
npm ERR! @angular/cdk@"^16.2.14" from the root project  
npm ERR! 9 more (@angular/forms, @angular/platform-browser, ...)  
npm ERR!  
npm ERR! Could not resolve dependency:  
npm ERR! peer @angular/common@"^15.0.0" from @nebular/auth@11.0.0  
npm ERR! node_modules/@nebular/auth  
npm ERR! @nebular/auth@"^11.0.0" from the root project  
npm ERR!  
npm ERR! Conflicting peer dependency: @angular/common@15.2.10  
npm ERR! node_modules/@angular/common  
npm ERR! peer @angular/common@"^15.0.0" from @nebular/auth@11.0.0  
npm ERR! node_modules/@nebular/auth  
npm ERR! @nebular/auth@"^11.0.0" from the root project  
npm ERR!  
npm ERR! Fix the upstream dependency conflict, or retry  
npm ERR! this command with --force or --legacy-peer-deps  
npm ERR! to accept an incorrect (and potentially broken) dependency resolution.  
npm ERR!  
npm ERR!  
npm ERR! For a full report see:  
npm ERR! /Users/mathieuleprovost/.npm/_logs/2024-03-19T13_31_22_124Z-eresolve-report.txt  

  

  

Cette erreur se produit lorsque npm essaie de résoudre les dépendances pour installer un package, mais qu'il rencontre des conflits entre les versions des packages requis par différents modules.

Dans ton cas, l'erreur indique que tu as deux dépendances qui requièrent différentes versions de `**@angular/common**` :

1. `**@nebular/auth@11.0.0**` nécessite `**@angular/common@^15.0.0**`.
2. `**@angular/cdk@16.2.14**` nécessite `**@angular/common@^17.3.0**`.

Cela crée un conflit, car npm ne sait pas quelle version de `**@angular/common**` utiliser.

Pour résoudre ce problème, tu as quelques options :

1. **Fixer le conflit de dépendance :** Dans certains cas, il est possible de mettre à jour les versions des packages afin qu'ils utilisent tous la même version de la dépendance. Cependant, cela peut ne pas être possible ou souhaitable en fonction des exigences du projet.
2. **Forcer l'installation :** Tu peux utiliser l'option `**-force**` ou `**-legacy-peer-deps**` lors de l'exécution de la commande `**npm ci**` pour forcer npm à installer malgré les conflits. Cependant, cela peut entraîner des problèmes de compatibilité ou de fonctionnalité entre les packages.
3. **Analyser les logs pour plus d'informations :** Les logs de npm peuvent fournir des informations supplémentaires sur les dépendances en conflit et les raisons pour lesquelles elles sont nécessaires. Cela peut aider à comprendre la nature du problème et à décider de la meilleure approche pour le résoudre.

Dans tous les cas, assure-toi de prendre des décisions en fonction des besoins spécifiques de ton projet et de tester attentivement les changements pour éviter d'introduire des problèmes inattendus

  

npm WARN deprecated @npmcli/move-file@2.0.1: This functionality has been moved to @npmcli/fs