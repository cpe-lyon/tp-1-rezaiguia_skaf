# Compte Rendu TP1
## Rezaiguia Sarah - Skaf Paul

### Exercice 2: Prise en main de l’interpréteur de commandes 

#### Manuel 

1) Which permet de localiser le chemin d'un exécutable associé à la commande passé en argument, exemple : 

>which python 

>'/usr/bin/python' 


2) Pour rechercher un terme dans le manuel, on utilise "/" pour repérer un "pattern" , exemple : 

>/option 

*permet de trouver le mot option dans le manuel une fois ouvert*

3) Pour quitter le manuel on appuie sur "q" 

4) La section 6 du manuel présente les programmes "amusants" et les jeux présents sur le système.

#### Navigation dans l’arborescence des fichiers 

Le dossier racine "root" n'est pas accessible par tous les utilisateurs. Pour y accéder, on doit utiliser la commande *Sudo cd /root* qui permet d'exécuter une commande avec des droits administrateurs.

Pour créer un dossier, on utilise la commande *mkdir nomdudossier*, pour supprimer un dossier on utilise la commande *rmdir nomdudossier*.

Pour créer un fichier, on utilise la commande *touch nomdufichier*, et pour le supprimer : *rm nomdufichier*.

Pour supprimer un dossier vide, on utilise la commande *rmdir* . S'il n'est pas vide on utilise la commande *rm -r* qui va supprimer le contenu d'un dossier parent de manière récursive. 


#### Commandes Importantes

Afin d'afficher l'heure, on utilise la commande *date*. La commande *time* permet de mesurer le temps d'exécution de la commande qui sera donné en argument, exemple : 
> time mkdir dossier1

Pour afficher le contenu du répértoire courant, on utilise *ls*.
De plus, *la* affiche également les dossiers cachés.
La commande ls se situe dans */usr/bin/ls* .
La commande *ll* est en fait un alias de la commande *ls -l *. *Alias* permet de créer des "raccourcis" de commande personnalisés.
La commande *ls /bin* permet d'afficher le contenu du répertoire /bin.
La commande *ls* énumère les fichiers et dossiers présents dans le répertoire courant.
La commande pwd permet d'afficher le répertoire courant.

N'importe quelle commande suivie du chevron redirige la sortie de cette commande dans un fichier donné en argument après le chevron, exemple : 
> echo 'yo' > plop

> Cette commande va écrire "yo" dans le fichier plop. Si cette commande est exécutée 2 fois, on remplace le fichier plop par la nouvelle sortie de la commande. Pour écrire à la suite il faut mettre deux chevrons *echo 'yo' >> plop*.

La commande *file* permet de déterminer le type d'un fichier 

Lorsqu'on crée un lien avec la commande *ln toto titi* et qu'on modifie toto, le lien titi est également modifié. La suppression de toto n'entraîne pas la suppressin de titi.

Si on crée un lien symbolique, la suppression de toto entrînera celle de titi.

Le raccourci ctrl+c permet de terminer le défilement en cours.

Pour afficher les 5 premières lignes d'un fichiers, on utilise la commande *head -n 5 fichier*
Pour afficher les X dernières lignes d'un fichier, on utilise la commande *tail -n X fichier*
Pour afficher de la ligne a à la ligne b on utlise : *sed -n a,bp fichier*





