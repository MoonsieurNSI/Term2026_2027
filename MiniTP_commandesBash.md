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

**Question 2.** Afficher la liste des fichiers et dossiers présents dans le répertoire courant.

**Question 3.** Afficher cette liste en incluant les fichiers cachés et les informations détaillées (permissions, propriétaire, taille, date de modification).

**Question 4.** Se déplacer dans le répertoire `/home`, puis revenir dans son répertoire personnel.

**Question 5.** Afficher l'arborescence des fichiers et dossiers présents dans votre répertoire personnel. Si la commande `tree` n'est pas installée, utiliser une autre méthode.

## Partie 2 – Créer et organiser des fichiers

**Question 6.** Dans votre répertoire personnel, créer un dossier nommé `MiniTP_Linux`.

**Question 7.** Se placer dans ce dossier et y créer les trois sous-dossiers suivants :
- `Documents`
- `Images`
- `Scripts`

**Question 8.** Dans le dossier `Documents`, créer deux fichiers vides nommés `cours.txt` et `notes.txt`.

**Question 9.** Afficher le contenu du dossier `Documents` pour vérifier que les deux fichiers ont bien été créés.

**Question 10.** Copier le fichier `cours.txt` dans le dossier `Scripts`. Renommer ensuite cette copie en `programme.py`.

**Question 11.** Déplacer le fichier `notes.txt` dans le dossier `Images`.

## Partie 3 – Manipuler le contenu des fichiers

**Question 12.** À l'aide de la commande `echo`, écrire le texte suivant dans le fichier `cours.txt` :

`Linux est un système d'exploitation.`

Puis ajouter une deuxième ligne :

`Le terminal permet de communiquer avec le système.`

*Indication :* utiliser les opérateurs `>` et `>>`. Quelle est la différence entre ces deux opérateurs ?

**Question 13.** Afficher le contenu du fichier `cours.txt` à l'aide de la commande `cat`.

**Question 14.** Afficher le contenu du fichier `cours.txt` page par page à l'aide de la commande `less`. Quelle touche permet de quitter cet affichage ?

**Question 15.** À l'aide de la commande `grep`, rechercher le mot `terminal` dans le fichier `cours.txt`.

**Question 16.** Utiliser la commande `wc` pour compter :
- le nombre de lignes du fichier ;
- le nombre de mots ;
- le nombre de caractères.

## Partie 4 – Utilisateur et système

**Question 17.** Utiliser les commandes appropriées pour :
- afficher le nom de l'utilisateur actuellement connecté ;
- afficher ses identifiants et ses groupes ;
- afficher le chemin de l'exécutable Python installé sur le système.

**Question 18.** Afficher l'historique des dernières commandes saisies dans le terminal.

---

## Pour aller plus loin

1. À l'aide de la commande `chmod`, rendre le fichier `programme.py` exécutable. Quelle commande permet de vérifier que les permissions ont bien été modifiées ?

2. Supprimer les fichiers et les dossiers créés pendant ce TP. Commencer par supprimer les fichiers, puis les dossiers vides.

3. Quelle est la différence entre les commandes `rm`, `rmdir` et `rm -r` ?

