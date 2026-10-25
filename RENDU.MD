# Rendu : AdrienLiossatos

- Dépôt : https://github.com/AdrienLiossatos/tp-git-qqch 
- Site GitHub Pages : https://adrienliossatos.github.io/tp-git-qqch/  

## Ex2
git log --oneline : (base) adrien@MacBook-Air-de-LIOSSATOS tp-git-qqch % git log --oneline
    8c2bb6d (HEAD -> main, origin/main) ex2 : corrige une faute
    55f8b8d ex2: crée les notes
    a7208fc ex1: initialise le dépôt 

## Ex3
- config.local est-il encore dans l'historique ? Pourquoi ?
  Normalement oui car avant le gitignore je l'ai bien commité.

## Ex4
- git status après avoir retiré brouillon.txt du staging : On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   brouillon.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.DS_Store

no changes added to commit (use "git add" and/or "git commit -a") 

- Différence entre annuler une modification et retirer du staging ?

  Retirer du staging signifie simplement que le fichier modifié n'attends pas de commit (il est avant le stade du git add), mais que sa modification existe au niveau local ; tandis qu'annuler une modification écrase tout modification non sauvegardée et redonne l'état initial du fichier modifié.

## Ex6
- À quoi servent <<<<<<<, ======= et >>>>>>> ?

  Il s'agit de marqueurs de conflits qui indiquent les endroits où deux branches merged rentrent en opposition. Ce sont des marqueurs visuels qui aident l'éditeur à corriger le(s) conflit(s) afin de pouvoir merge correctement.

## Ex7
- git stash list (avant récupération) : stash@{0}: WIP on main: 7cad9bc Revert "ex7 : ajoute une ligne par erreur"
stash@{1}: WIP on main: 7cad9bc Revert "ex7 : ajoute une ligne par erreur"
stash@{2}: WIP on main: 7cad9bc Revert "ex7 : ajoute une ligne par erreur"
- Pourquoi annuler un commit plutôt que l'effacer de l'historique ?

  Car cela permet de tracer l'évolution du projet collectif : on remplace l'ancien commit par un nouveau mais une trace est laissée. Tandis que le supprimer tout bonnement de l'histoire efface complètement toute trace de changement, ce qui est préjudiciable auprès des autres personnes qui travaillent sur le projet.

## Ex8
- git pull = git fetch + quoi ?

  git pull = git fetch + git merge

## Ex10
git log --oneline --graph --all : 

(base) adrien@MacBook-Air-de-LIOSSATOS tp-git-qqch % git log --oneline --graph --all
* ee4bbea (HEAD -> main, origin/main, origin/HEAD) correction lien repo sur site github pages
* 07daef3 ex9 : 2e ajout de l'url du site github pages sur le rendu
* 4ec4472 ex9 : ajout de l'url du site github pages dans readme et rendu
* 0165ccb ex 9 : ajoute la page d'accueil
* f00da95 Fix typo in README and add modification note
*   2a1b903 Merge pull request #1 from AdrienLiossatos/feature-contact
|\  
| * 2685dbb (origin/feature-contact, feature-contact) ex8 : ajoute la page contact
|/  
* 4242f2c rendu stash ex7
| *   85bd739 (refs/stash) WIP on main: 7cad9bc Revert "ex7 : ajoute une ligne par erreur"
|/|\  
| | * 3085315 untracked files on main: 7cad9bc Revert "ex7 : ajoute une ligne par erreur"
| * c91718f index on main: 7cad9bc Revert "ex7 : ajoute une ligne par erreur"
|/  
* 7cad9bc Revert "ex7 : ajoute une ligne par erreur"
* 73480ef ex7 : ajoute une ligne par erreur
*   48e1cf6 ex6 : résout le conflit du titre
|\  
| * d91bcef (origin/version-en) ex6 : titre en anglais
* | dd1b8d0 (origin/version-fr) ex6 : titre en français
|/  
*   2b0d5c1 ex5 : fusionne feature-menu
|\  
| * 0771b6f (origin/feature-menu) ex5 : ajoute un dessert
| * cf4f3ea ex5 : créé le menu
|/  
* 92dc97e ex4 : ajout du rendu
* ff37754 ex4 : supprime a-supprimer.txt





