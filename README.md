# Tutoriel

Dans ce Tuto on apprend à mettre en place un environnement de travail, créer des répertoires et des fichiers.

## 1. Créer un fichier:

``` touch index.html ```

Dans l'éditeur de texte par exemple atom on écris le code:

``` <!doctype html>
<html lang="en">
	<head>
		<meta charset='UTF-8">
		<meta name='viewport"
			content="width=device-width, user-scalable=no,
initial-scale=1.0, maximum-scale=1.0, minimim-scale=1.0">
		<meta http-equiv="X-UA-Compatible" content="ie=edge">
		<title>Document</title>
		<link rel="stylesheet" href="style.css">
	</head>
	<body>
</html> ```

 ## 2. Initialiser le code sur GitBash, en utilisant la commande:

 ``` git init ```

Cette commande va créer un dossier caché ```.git```  si on ne lo vois pas. On peut y aller dans l'explorateur windows et ouvrir l'onglet ```views``` ou ```Affichage```, ensuite click sur ```option``` dans Cette fenêtre selectionner ```view``` ou ```affichage``` et selectionner l'option : "Afficher les fichiers, dossiers et lecteurs cachés".

## 3. Envoyer les informations sur le GitHub.

S'identifier sur le GitBash, name, username:

``` git config --global user.name 'ttt' ```

``` git config --global user.email 'ttt@gmail.com' ```

## 4. Ajouter le fichier index.html avec la commande:

``` git add index.html ```

Cette commande va aussi servir a faire une pre-sauvegarde.

## 5. Visualiser la pre-sauvegarde:

``` git status ```

## 6. On confirme cette sauvegarde:

``` git commit ```

## 7. si on veut retirer un fichier de cette sauvegarde, on utilise la commande:

``` git rm --cached index.html ```

attention il faut mettre les deux tirés si non on elimine les fichiers.

## 8. Si on veut ajouter un fichier .css:

``` touch style.css ```

## 9. Ajouter tous les fichiers présents dans un dossier:

``` git add . ```

## 10. Si on veut retirer un fichier qui est apparu et qu'on voulait ignorer, on fait:

``` git rm -r --cached .idea/ ```

l'option r est pour suprimer recursivement tous les fichier à l'intèrieur.

## 11. Si on veut retirer tous les fichiers cache recursivement du dossier où nous nous trouverons:

``` git rm -r --cached. ```

## 12. On ajoute les differents extension qu'on souhaite:

``` git add *.html *.css ```

## 13. Si on a supprimé quelque fichier, on peut le récuperer avec la commande:

``` git checkout ```

## 14. On sauvegarde en ajoutant un message:

``` git commit -m 'nom du changement' ```

## 15. Créer un fichier gitignore:

``` touch .gitignore ```

Dans l'editeur de texte on écris les fichiers que l'on souhaite ignorer.

## 16. Créer une branche:

``` git branch fichierJS ```

note: par l'instant rien n'a changé on est toujours dans la branche principale.

## 17. Changer de branche:

``` git checkout fichierJS ```

## 18. Se rappeler des noms des branches:

``` git branch --list ```

## 19. En étant sur la branche 'fichierJS'. Créer un fichier par example main.js:

``` touch main.js ```

dans l'éditeur de texte en main.js on écris le code. et dans le fichier index.html on ajoute les balises script.

## 20. On ajoute tout le dossier à nouveau:

``` git add . ```

## 21. On fait un commit:

``` git commit -m 'Ajout du fichier JS' ```

## 22. Passer sur la branche principale:

``` git checkout master ```

## 23. Fusionner la branche dans la branche principale master:

``` git merge fichierJS ```

fichierJS: c'est le nom de la branche.

## 24. Aller sur GitHub:

Tout d'abord nous devons creer un repository sur GitHub. on selectionne l'option " push an existing repository from the command line".

On copie la suivante commande sur GitBash

``` git remote add origin https://github.com/users/nomderepository ```

Suivre les pas d'autenthification.

## 25. Créer un README à partir de GitBash:

``` touch README.md ```

``` git add . ```

``` git commit -m 'Ajout du fichier README' ```

ref: https://www.youtube.com/watch?v=4o9qzbssfII
