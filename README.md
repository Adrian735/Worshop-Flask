# Worshop flask 
- Adrian Lorenzi / Anthony Ghizzo 
- 2021-2022

## Objectif
Apprendre les bases de la création de site web en Python, avec le freamwork Flask

- Documentation Flask
https://flask.palletsprojects.com/en/2.1.x/

## Installation

- Mise en place de l'environnement virtuel
```shell
python3 -m venv Flask_workshop
source Flask_workshop/bin/activate
```

- Installer le freamwork flask
```shell
pip install Flask
```

- Exécuter flask
```shell
export FLASK_APP=main.py
export FLASK_ENV=development
flask run
```

## Workshop

- Step 1
Creer une route a l'index qui affiche "Hello world" 

- Step 2
Creer une route /profil/nom/age qui age "Bonjour ... vous avez ... ans."

- Step 3
Creer une route /image qui affiche l'image Flask.png contenu dans le repo

- Step 4
Creer une route /user qui permet d'afficher un template user.html
Ce template utilisera Jinja et permet affiche dynamiquement les info des utilisateur contenu dans le fichier user.py (prénom, nom et age)

- Step 5
Creer une route /login qui affiche une page index.html contenant un formulaire.
Si l'username et le password correspondent à "admin", l'utilisateur est redirigé vers la page user.html
sinon le message "accès refusé" est affiché.

- Step 6
Implémenter des sessions, Le but des sessions est de sécuriser l'accès aux pages web du site.
Tout utilisateur non connecté et souhaitant accéder à l'une des pages web du site se verra rediriger vers la page login.
Egalement implémenter une route /logout permettant de déconnecter l'utilisateur

## Bonus

- Implémenter une page header.html et footer.html que l'on incluera sur chacune des pages crée précédement
- Améliorer le front du site en utilisant un freamwork web (Bootstrap par exemple)