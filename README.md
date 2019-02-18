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

Créez les dummy users :

`bin/console doctrine:fixtures:load`

