Quete Git Remote Wild Code School

Challenge

Envoi ton code sur github

Pour commencer fait un

git status
Afin de t'assurer que tu n'as pas de fichiers non "addés" (c'est à dire modifié dans ton répertoire de travail mais pas dans l'index)

Si tu n'es pas à jour, ajoute les fichiers qui ne le seraient pas (et qui doivent l'être), puis commit tes modifications.

Ensuite, on suppose que ton travail dans la branche wcs est fini, testé et correct. Donc tu dois le réintégrer dans la branche master. Pour cela, tu as plusieurs solutions mais pour cette quête nous allons utiliser un merge sans option particulière.

Rend toi sur la branche master et met la à jour :

git checkout master
git pull origin master
Question : connais tu une autre façon de faire pour arriver au même résultat que le pull ?
Maintenant tu dois "merger" la branche wcs dans master, pour cela :

git merge wcs
Dans le cas ou tu n'as que des ajouts (c'est le cas ici). Tu n'auras aucun soucis. Par contre si un fichier présent dans la branche master a été modifié dans la branche wcs sur une ligne déjà existante, Git te demandera de régler le conflit manuellement. Concrètement il va te proposer les 2 versions, celle de la branche wcs et celle de la branche master, à toi de choisir laquelle est correcte (discute avec ton équipe car master a pu évolué).

Rends toi sur Github dans l'onglet "code" et soumet cette url dans odyssey.

Critéres de validation

La branche master doit contenir le fichier wild.php
