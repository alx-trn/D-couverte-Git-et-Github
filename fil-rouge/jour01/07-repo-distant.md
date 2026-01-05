# je veux partager mon code sur un dépôt distant 

- prendre mon code est le mettre sur github 
- je dois me connecter github (avec un profil)
- créer un répository sur github (le nom du projet)
- copier les commandes suivantes 

```sh
# associer le repository local avec le resposity distant 
git remote add origin <adresse de votre repository>


# prendre l'ensemble des commits enregistrés dans votre ordinateur
# et les envoyer (push) sur le repository distant 
git push -u origin main
```
# Cas pratique

Dans le fichier index.html ajouter à la fin du fichier dans la page footer un formulaire avec 2 champs;
    - Un champ input de type email qui permet à l'utilisateur de s'inscrire à newslatter
    - Un button pour soumettre le formulaire

Une fois que le code est saisie vous allez faire :
git add .
git commit -m "feat(home) formulaire newslatter"
git push

Regarder sur le github si le commit a bien été ajouté

---

# Git remote

- Permet de faire une liaison entre les REPO local et le REPO distant

```sh
git remote add origin <adresse_internet>
```

Connaitre l'adresse de mon dépôt

```sh
git remote --verbose
git remote -v
```

- push LOCAL -> DISTANT
- push DISTANT -> LOCAL

# Je veux changer l'adresse du dépôt distant

- Solution 1:
    - Supprimer l'adresse et refaire un git remote add

```sh
git remote rm origin
git remote add origin <nouvelle_adresse_internet>
```