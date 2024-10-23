1. Modes de Vim :

2. Naviguer dans Vim :

3. Éditer du texte :

4. Enregistrer et quitter :

5. Rechercher et remplacer :

6. Indenter :

7. Sauvegarder et quitter rapidement :

Résumé rapide des principales étapes pour modifier un fichier dans dom0 avec Vim :

Voici un ensemble des **commandes élémentaires de Vim** qui te permettront d’éditer des fichiers directement depuis **dom0** :

### 1. **Modes de Vim** :

- **Mode normal** (ou commande) : Le mode par défaut pour naviguer et exécuter des commandes. Appuie sur `Esc` pour y revenir à tout moment.
- **Mode insertion** : Permet de taper et modifier le texte. Utilise les commandes comme `i` pour entrer dans ce mode.
- **Mode commande** : Permet d’exécuter des commandes de fichier, comme sauvegarder ou quitter. Tape `:` pour entrer dans ce mode depuis le mode normal.

### 2. **Naviguer dans Vim** :

- `h`, `j`, `k`, `l` : Se déplacer à gauche, en bas, en haut et à droite, respectivement.
- `gg` : Aller au début du fichier.
- `G` : Aller à la fin du fichier.
- `w` : Avancer d’un mot.
- `b` : Reculer d’un mot.
- `0` : Aller au début de la ligne.
- `$` : Aller à la fin de la ligne.

### 3. **Éditer du texte** :

- `i` : Entrer en **mode insertion** avant le curseur.
- `a` : Entrer en **mode insertion** après le curseur.
- `o` : Ajouter une nouvelle ligne en dessous et entrer en **mode insertion**.
- `O` : Ajouter une nouvelle ligne au-dessus et entrer en **mode insertion**.
- `x` : Supprimer le caractère sous le curseur.
- `dd` : Supprimer (couper) la ligne entière.
- `yy` : Copier la ligne entière.
- `p` : Coller après le curseur.
- `u` : Annuler la dernière action.
- `Ctrl + r` : Rétablir une action annulée.

### 4. **Enregistrer et quitter** :

- `:w` : Sauvegarder le fichier.
- `:q` : Quitter Vim.
- `:wq` ou `:x` : Sauvegarder et quitter.
- `:q!` : Quitter sans sauvegarder.

### 5. **Rechercher et remplacer** :

- `/motif` : Rechercher un texte dans le fichier. Tape `/` suivi de ton motif (ex. `/config`) puis `Entrée`.
- `n` : Aller à l’occurrence suivante.
- `N` : Aller à l’occurrence précédente.
- `:%s/motif/texte/g` : Remplacer tout le motif par le texte donné dans tout le fichier. Par exemple, `:%s/ancien/nouveau/g`.

### 6. **Indenter** :

- `>>` : Indenter la ligne actuelle.
- `<<` : Désindenter la ligne actuelle.

### 7. **Sauvegarder et quitter rapidement** :

- **Écrire et quitter** : `:wq` ou `ZZ`
- **Quitter sans écrire** : `:q!` ou `ZQ`

### Résumé rapide des principales étapes pour modifier un fichier dans dom0 avec Vim :

1. **Ouvrir le fichier** : Depuis dom0, utilise la commande :
    
    ```Shell
    bash
    Copy code
    vim ~/.config/i3/config
    
    ```
    
2. **Naviguer et éditer** :
    - Tape `i` pour entrer en **mode insertion** et commencer à modifier le fichier.
    - Une fois les modifications faites, tape `Esc` pour revenir en **mode normal**.
3. **Sauvegarder et quitter** :
    - Tape `:wq` pour sauvegarder et quitter Vim.

Ces commandes te permettront de naviguer efficacement dans un fichier et de le modifier directement depuis **dom0** en utilisant **Vim**.