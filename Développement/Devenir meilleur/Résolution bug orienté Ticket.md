  

Phase 1 : Identifier le bug

Etape 1 : Reproduire le bug

Étape 2 : Comprendre le bug

Étape 3 : Comprendre le comportement attendu

Étape 4 : Délimiter le problème

Étape 5 : Auditer le code

Phase 2 : La correction du bug

Étape 6 : Mettre en œuvre la correction

Étape 7 : Tester la correction

Étape 8 : Nettoyer le code

Étape 9 : Signaler le bug

Sources :

## **Phase 1 : Identifier le bug**

### **Etape 1 : Reproduire le bug**

- Recueillir le maximum d’informations sur l’état du système au moment où le bug s’est produit ⇒ Afin de recopier l’environnement dans lequel ce bug s’est produit et l’identifier correctement.
    - Voir Logs pour savoir ce qui a mal tourné
    - Demander à la personne qui a détecté le bug

⇒ Aide à comprendre le bug et même savoir s’il a été corrigé ou non

### **Étape 2 : Comprendre le bug**

- Savoir qu’il y a une erreur et la comprendre sont deux choses différentes.
    - ⇒ Comprendre exactement pourquoi les choses ne fonctionnent pas comme on le souhaite. Autrement dit quel est la cause précise de ce bug

### **Étape 3 : Comprendre le comportement attendu**

- Être certains de l’objectif que l’on vise
    - Quel comportement vise-t-on exactement
    - Voir documentation / cahier des charges / chef de projet / client
    - voir si le bug est réellement prioritaire
    - voire s’il existe réellement

### **Étape 4 : Délimiter le problème**

⇒ étape itérative = par tâtonnements en entonnoir.

- Localiser la partie du code qui provoque le bug.
    - Utilisez les logs
    - Ajoutez des logs s’ils n’existent pas
    - utilisation débuger
    - refactorisation du code pour le clarifier
    - Testez ⇒ TI afin de permettre de délimiter le problème
    - pour savoir si x est dysfonctionnel et donc responsable du bug : comprendre le comportement attendu ⇒ observer le comportement réelle
- ⇒ Si le problème est difficile à délimiter, c’est certainement que l’app a des problèmes conceptuels ou architecturaux.

⇒ A cet endroit le bloc de code qui pose problème doit être identifié

### **Étape 5 : Auditer le code**

- **inspecter les autres parties du code** (fonctions, modules, etc.) **en interaction avec lui** pour les raisons suivantes :
    - Ces parties peuvent **être la source du problème**
    - La cause de votre bug dans le bloc de code identifié peut **avoir le même effet sur les blocs en interaction**.
    - La correction que vous avez l’intention de mettre en œuvre peut **avoir des effets secondaires sur ces parties**.

## **Phase 2 : La correction du bug**

### **Étape 6 : Mettre en œuvre la correction**

- corrigez le bug identifié ⇒ à détailler

### **Étape 7 : Tester la correction**

- reproduire les conditions qui ont conduit au bug
    - et de confirmer que, cette fois, plutôt que d’avoir le bug,
    - vous avez le comportement attendu.
- valider qu’aucune régression n’a résulté de la correction

⇒ régression = changement dans le code qui crée un bug autre part

- Exploiter l’audit de l’étape cinq pour écrire les tests adéquats.
    - Il est important de faire un test ici car si le bug est apparu et qu’il a été difficile à identifier c’est qu’il manque un TI
    - écrire les test permet d’éviter les régressions et l’apparition d’autre bugs
    - rappel : test coverage 100% ne couvre pas TOUS les cas possible

### **Étape 8 : Nettoyer le code**

- Améliorer l’état du code avec
    - des logs ( s’ils n’existaient pas )
    - CHECK SOLID surtout : SO
    - formattage + lisibilité

⇒ Faire tout son possible pour avoir un code de qualité simple à tester, débuger, maintenir, implémenter

### **Étape 9 : Signaler le bug**

- générez un rapport de bug contenant :
    - la **description** du bug,
    - les **causes** de celui-ci,
    - le **comportement attendu**,
    - la **résolution**.
- Objectif :
    - ⇒ permet de pouvoir facilement re résoudre le bug s’il se reproduit
    - ⇒ permet aussi de déléguer la résolution du bug à d’autre membres de l’équipe

### Sources :

[Codeur.com](https://www.codeur.com/blog/meilleure-methode-resoudre-bug/) ⇒ [developpez.com](https://programmation.developpez.com/actu/88641/La-correction-de-bug-en-7-etapes-par-GeoffreyOnRails/)