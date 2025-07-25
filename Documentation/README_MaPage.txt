README - Mettre à jour votre site GitHub Pages depuis VS Code
===========================================================

Objectif :
----------
Ce fichier vous guide pas à pas pour publier ou mettre à jour votre site web hébergé sur GitHub Pages depuis votre dossier local (VS Code), sans jamais supprimer le dépôt GitHub.

Dépôt utilisé :
---------------
URL : https://github.com/NicodemeKONE/Page
Branche principale : main
Page web : https://nicodemekone.github.io/Page/

Prérequis :
-----------
✅ Git installé sur votre ordinateur
✅ VS Code installé
✅ Un compte GitHub actif
✅ Un dépôt GitHub existant
✅ Une version locale de votre site (fichiers HTML/CSS/JS)

Étapes détaillées :
-------------------

1. Ouvrir le bon dossier dans VS Code
--------------------------------------
Exemple de dossier : C:\Users\eunic\OneDrive\Documents\NICODEME\MaPage

2. Initialiser Git (à faire une seule fois)
-------------------------------------------
Dans le terminal VS Code :
    git init

3. Lier ce dossier au dépôt GitHub
-----------------------------------
    git remote add origin https://github.com/NicodemeKONE/Page.git

4. Ajouter tous les fichiers
----------------------------
    git add .

5. Créer un commit (enregistrer les changements)
------------------------------------------------
    git commit -m "Mise à jour du site"

6. Forcer l'envoi vers GitHub (main = branche principale)
---------------------------------------------------------
    git push -f origin main


⚠️ Si une erreur 403 apparaît :
-------------------------------
Cela signifie que Git utilise le mauvais compte GitHub (ex : eunicelamah).

Solution :
- Générez un token GitHub ici : https://github.com/settings/tokens
  > Cliquez sur "Generate new token (classic)"
  > Cochez "repo", choisissez une durée, et générez
  > Copiez le token

- Puis remplacez l'URL distante :
    git remote set-url origin https://TON_TOKEN@github.com/NicodemeKONE/Page.git


- Ensuite :
    git push -f origin main

- Remettez l'URL propre :
    git remote set-url origin https://github.com/NicodemeKONE/Page.git

7. Vérifier que le site est en ligne
-------------------------------------
Allez sur : https://nicodemekone.github.io/Page/

8. Modifier votre site
-----------------------
- Faites les modifications dans VS Code
- Puis relancez :
    git add .
    git commit -m "Votre message"
    git push

cd "C:\Users\eunic\OneDrive\Documents\NICODEME\MaPage"
git add .
git commit -m "Votre message ici"
git push


Et votre site sera mis à jour !

Fichier généré automatiquement le : 2025-07-25