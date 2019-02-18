# Symfony Blog

## Installation et préparation du projet

Pour installer et démarrer ce projet Symfony, créez une base de données mysql nommée "blog". Créez ensuite un utilisateur 
"symfony" ayant pour mot de passe "123456" avec les accès à cette base.

Récupèrez ensuite le projet :

`git clone https://github.com/ig1na/SymfonyBlog.git && cd SymfonyBlog`

Installez les dépendances composer :

`composer install`

Installez les dépendances node :

`npm install`

Créez les tables en faisant une migration :

`bin/console make:migration`\
`bin/console doctrine:migration:migrate`

Construisez les assets : 

`./node_modules/.bin/encore dev`

Créez les dummy users :

`bin/console doctrine:fixtures:load`

Lancez le serveur :
`bin/console server:start`

Pour créer/éditer/supprimer des articles, rendez-vous sur l'application et cliquez sur le bouton "login" dans le menu en haut. Connectez-vous avec le dummy user en renseignant l'email "admin@admin.fr" et le mot de passe "admin".
