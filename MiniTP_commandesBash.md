# Mini-TP – Les commandes de base sous Linux

**Objectif :** découvrir et maîtriser les principales commandes Linux en manipulant des fichiers et des dossiers depuis un terminal.

**Consignes :**
- Réaliser les manipulations directement dans un terminal Linux.
- Pour chaque question, noter la commande utilisée.
- Lorsque cela est demandé, expliquer brièvement le résultat obtenu.
- Attention : certaines commandes peuvent supprimer définitivement des fichiers !

---

## Partie 1 – Se repérer dans le système

**Question 1.** Ouvrir un terminal et afficher le chemin absolu du répertoire dans lequel vous vous trouvez.
`pwd`
**Question 2.** Afficher la liste des fichiers et dossiers présents dans le répertoire courant.
`ls` ou `tree`

**Question 3.** Afficher cette liste en incluant les fichiers cachés et les informations détaillées (permissions, propriétaire, taille, date de modification).
`ls -a`
**Question 4.** Se déplacer dans le répertoire `/home`, puis revenir dans son répertoire personnel.
 `cd /home` puis `cd /workspaces/Term2026_2027`
**Question 5.** Afficher l'arborescence des fichiers et dossiers présents dans votre répertoire personnel. Si la commande `tree` n'est pas installée, utiliser une autre méthode.
`ls -R`
## Partie 2 – Créer et organiser des fichiers

**Question 6.** Dans votre répertoire personnel, créer un dossier nommé `MiniTP_Linux`.
`mkdir MiniTP_Linux`
**Question 7.** Se placer dans ce dossier et y créer les trois sous-dossiers suivants :
- `Documents`
- `Images`
- `Scripts`

`cd ./MiniTP_Linux/` puis `mkdir Documents Images Scripts`
**Question 8.** Dans le dossier `Documents`, créer deux fichiers vides nommés `cours.txt` et `notes.txt`.
`touch Documents/cours.txt Documents/notes.txt`
**Question 9.** Afficher le contenu du dossier `Documents` pour vérifier que les deux fichiers ont bien été créés.
`tree`
**Question 10.** Copier le fichier `cours.txt` dans le dossier `Scripts`. Renommer ensuite cette copie en `programme.py`.
`cp Documents/cours.txt Scripts/programme.py`

**Question 11.** Déplacer le fichier `notes.txt` dans le dossier `Images`.
`mv Documents/notes.txt Images/notes.txt`
## Partie 3 – Manipuler le contenu des fichiers

**Question 12.** À l'aide de la commande `echo`, écrire le texte suivant dans le fichier `cours.txt` :

`Linux est un système d'exploitation.`

`echo "Linux est un système d'exploitation" >
 Documents/cours.txt`
Puis ajouter une deuxième ligne :

`Le terminal permet de communiquer avec le système.`

`echo "Le terminal permet de communiquer avec le système." >> Documents/cours.txt`
*Indication :* utiliser les opérateurs `>` et `>>`. Quelle est la différence entre ces deux opérateurs ? La double fèlche rajoute sans écraser le contenu

**Question 13.** Afficher le contenu du fichier `cours.txt` à l'aide de la commande `cat`.
`cat Documents/cours.txt `
**Question 14.** Afficher le contenu du fichier `cours.txt` page par page à l'aide de la commande `less`. Quelle touche permet de quitter cet affichage ?
`less Documents/cours.txt ` puis touche `Q`
**Question 15.** À l'aide de la commande `grep`, rechercher le mot `terminal` dans le fichier `cours.txt`.
 `grep "terminal" Documents/cours.txt` 
**Question 16.** Utiliser la commande `wc` pour compter :
- le nombre de lignes du fichier ;    `wc -l Documents/cours.txt `
- le nombre de mots ;   `wc -w Documents/cours.txt `
- le nombre de caractères. `wc -m Documents/cours.txt `

## Partie 4 – Utilisateur et système

**Question 17.** Utiliser les commandes appropriées pour :
- afficher le nom de l'utilisateur actuellement connecté ;  `whoami`
- afficher ses identifiants et ses groupes ;  `id`
- afficher le chemin de l'exécutable Python installé sur le système. `which python3`

**Question 18.** Afficher l'historique des dernières commandes saisies dans le terminal.
`history`
---

## Pour aller plus loin

1. À l'aide de la commande `chmod`, rendre le fichier `programme.py` exécutable. Quelle commande permet de vérifier que les permissions ont bien été modifiées ?
`chmod u+x,g-w,o-w Scripts/programme.py`
ou `chmod 700 Scripts/programme.py `

|valeur|permission|
|---|---|
|4|`r`|
|2|`w`|
|1|`x`|


2. Supprimer les fichiers et les dossiers créés pendant ce TP. Commencer par supprimer les fichiers, puis les dossiers vides.
`rm -r ./`

3. Quelle est la différence entre les commandes `rm`, `rmdir` et `rm -r` ?
 - `rm` pour les fichiers uniquement
 - `rmdir` pour les dossiers vides uniquement
 - `rm -r` pour tout
