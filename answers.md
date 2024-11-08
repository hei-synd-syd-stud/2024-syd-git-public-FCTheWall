# Answers of François Clément FCTheWall

## Basics
### Task 1
	- Un fichier .git faisant le lien entre l'emplacement local dans l'ordinateur ainsi que l'emplacement sur le web.
	- Des fichiers créés pour cet exercice, soient img et "answers.md"

### Task 2
	En faisant un git status, il y a maintenant une untracked file, soit README.md.
	Pour le git log --oneline, pas de différence.
	
	Pour le status, cela s'explique car il y a un nouveau fichier, pas seulement une modification.
### Task 3
	Après avoir effectué git add README.md, on voit bien qu'en faisant un git status, il n'y a plus de untracked file, c'est logique.

### Task 4
	En faisant un git status après la modification du README.md, on voit bien que dans les changements qui doivent être "commited" la new file : README.md est présente
	De plus, on voit aussi les changements "not staged" les deux fichiers .md, car les deux sont modifiés.

### Task 5
	Voici ce qu'on observe après avoir fait un commit puis un git log --online.
	- On a d'abord l'identifiant abrégé du commit au début de chaque ligne.
	- HEAD pointe sur le dernier commit de la branche main.
	- Après les parenthèses se trouve le message du commit, indiquant l'ajout d'un fichier README et l'Initial commit.

### Task 6
	Lorsqu'on fait un git checkout <idDuPremierCommit>, on perd le fichier README.md ET les modifications apportées au fichier answers.md.
	Et quand on revient sur le dernier commit, on voit les modifications revenir.
	Cela nous permet de revenir assez facilement sur des versions précédentes de notre projet.

## Gitgraph

	1 : Nom d'une branche, ici "develop".
	2 : Identifiant du commit, ici le dernier commit.
	3 : Message du commit pour décrire ce qui a été fait.
	4 : Identifiant de la personne ayant fait le commit.
	5 : Version de la branche principale (main).
	6 : Avancée actuelle de la branche "develop" où "feature-auth" vient de se merge.
	7 : branche feature-auth qui ajoute une fonctionnalité faite par une autre équipe que "develop", est ensuite merged quand elle est fonctionnelle.
	8 : Avancée actuelle de la branche "main", où un version de "develop" est mergée et d'où "feature-auth" part pour faire sa tâche.
	9 : Branche "develop" qui sert de branche de test avant de mettre la version finale de le main par exemple.
	10 : Branche main qui est la base du projet Git, mais aussi là où se terminera le projet quand tout sera fini.
	
### Task 7
	

![Gitgraph](img/gitgraph.svg)