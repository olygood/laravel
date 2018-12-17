# Laravel installation windows 10 pro
installation exercices laravel
## Installation  
### Première étape :  
> - Wamp server  
avec toutes les extensions chargées  
dans la doc de laravel https://laravel.com/docs/ il y a une version de php à respeceter ici : PHP >= 7.1.3
Server Requirements : 
- PHP >= 7.1.3
- OpenSSL PHP Extension
- PDO PHP Extension
- Mbstring PHP Extension
- Tokenizer PHP Extension
- XML PHP Extension
- Ctype PHP Extension
- JSON PHP Extension
- BCMath PHP Extension
#### tous les services si dessus doivent être présentes dans Wampserver.  
- dans wampserver qui tourne dans la barre de tache ou dans les icones caché allez dans :
- appache
  - Module appache
  - rewrite_module doit être activé.  
  ### deuxième étape :  **_IMPORTANT_**
regarder si PHP est bien installé en GLOBALE sur votre machine :
> - si vous avez installez wamp sans la commande _administrateur_
>- pour verifier allez dans le repertoir php dans Wamp: C:\wamp64\bin\php\php7.2.10  
- une fois localiser faite un clic sur php.exe 
- clic droit dans la barre d'adresse pour _copier en tant que texte_  l'adresse de l'exécutable  
- allez dans windows paramètres   
- et dans la barre de recherche tapez env (pour environemnt)
- variable d'utilisateur olivier
- et sélectionnez modifier les variables d'environement système  
- clic sur variable d'environement
- la variable que je dois modifier c'est la variable path
- clic sur path 
- modifier
- copier l'adresse que vous avez copier de php7.2.10 :C:\wamp64\bin\php\php7.2.10 
- soit à la suite ou derière un chemin existant donc la ajouter ';' deriere le chemin eistant et ';' a la fin du copié.
- ok fermer tout 
- pour s'assurer que le chemin à bien été copié en global 
- terminal 
- php - v
- et la vous avez la version de php.
### troisième étape :
## Installer _COMPOSER_  
va nous laisser manager les dépendances et télécharger directement les bibliothèques que d'autres auront dévelopés 
afin d'en profité dans notre projets  
- télécharger  :getcomposer.org download
- windows installer : composer-setup-exe
- pas coché dev contrôle 
- rechercher le chemin du php.exe 
- pas de proxy
- finish  
### Terminal
- composer -v
##installer Laravel : 
> - cibler le dossier auquel on veut travailler 
- on travaille avec wamp server et tous les dossier seront installer dans c:\ wamp64\wwww.  
- donc on va diriger l'invite de commante vers ce dossier  
- cd c:/wamp/www
- tapez la commande :
- composer create-project --prefer-dist laravel/laravel nomduprojet  
- composer télécharge laravel et créer le projet et il nous a installer notre application laravel
### ce connecter à laravel :
- si on fait localhost:8000/nomduprojet/ ca ne fonctionne pas pour ce connecter à laravel on doit cliquer sur public
- localhost:8000/nomduprojet/public/
- quel est le premier endroit on l'on doit commencer à travailler?
- tous ce qui est dans le dossier "app".


 


  
