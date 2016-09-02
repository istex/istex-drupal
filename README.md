# istex-drupal

Module Drupal 7 ayant pour vocation de permettre l'intégration des ressources ISTEX dans un environnement Drupal.  
Le module utilise les widgets ISTEX-SNU disponibles [ici](https://github.com/istex/istex-widgets-angular).  

## Installation

Téléchargez le fichier "istex-drupal-master.zip".  
Dé-zippez le fichier et placez le dossier istex_snu dans l'espace où vous mettez généralement les modules dans votre arboressence.  
Par exemple : /var/www/sites_drupal/sites/drupal.univ.fr/modules  
Connéctez-vous en tant qu'Administrateur à votre site Drupal.  
Cliquez sur "Modules" dans le menu Admin et tapez "istex" dans la barre "Filter list" puis activez le module et enregistrez la configuration.  


## Configuration
Les widgets peuvent être paramétrés en utilisant le menu de configuration.  
Cliquez sur "Modules" dans le menu Admin et tapez "istex" dans la barre "Filter list" puis cliquez sur "configurez".  

Les champs sont les suivants :
* Adresse du reverse proxy :
	C'est l'adresse par laquelle doivent passer les requêtes des utilisateurs. Souvent l'adresse correspond à un EZProxy.
* Facettes :
	C'est la liste des facettes (filtres de recherche) que vous voulez afficher.
* Recherche avancée :
	Dé-cochez la case si vous ne voulez pas afficher la recherche avancée.
* Pagination :
	Vous pouvez afficher une pagination en bas et/ou en haut de la page.
* Nombre de documents par page :
	C'est le nombre de résultats que vous voulez afficher par page.
* Requête par défaut :
	Vous pouvez lancer automatiquement une requête au chargement de la page (laissez la case vide si ça ne vous intéresse pas).

N'oubliez pas de cliquer sur "Enregistrer la configuration" !
	
## Placement des blocs

Une fois le module installé et configuré, survolez "Structure" et cliquez sur "Blocs".  
Vous verrez l'apparition de 3 nouveaux blocs dans la zone "Désactivé".  
Vous pouvez mettre ces blocs dans les zones que vous voulez, ou même ne pas les mettre (Seul le bloc "ISTEX-SNU results" est indispensable).  

Conseil : vous pouvez créer une page vide dédiée aux widgets et ne faire apparaître les blocs que sur cette page.  
Conseil 2 : le plus ergonomique est de mettre "Istex-snu search" dans "Menu", "Istex-snu facets" dans "Sidebar First" et "Istex-snu results" dans "Contenu".  

## Personnalisation de l'aspect visuel

Si vous voulez modifier l'aspect visuel des blocs pour harmoniser les couleurs avec le thème de votre université, vous avez à votre disposition le fichier istex_drupal.css.  
Le fichier se trouve dans istex_snu/css, à côté de style.min.css (le design par défaut).  
istex_drupal.css est vide, à l'exeption de sélécteurs pour vous guider et c'est à vous de le remplir pour répondre à vos besoin.  
Nous sommes bien sûr à votre disposition si vous avez besoin d'aide pour avoir le rendu souhaité.  

## Mise à jour du module

Pensez à faire une copie de istex_drupal.css.  
Ensuite, remplassez l'ancien dossier istex_snu par le nouveau.  
Enfin, écrasez istex_drupal.css avec la copie que vous avez faites.  

## Drupal 6 et Drupal 8

Le module n'a pas été testé sur les versions 6 et 8 de Drupal, nous ne pouvons donc pas garantir qu'il fonctionne dans ces cas précis.  
Si vous êtes dans un de ces deux cas, vous pouvez [nous contacter](mailto:istex-contact@univ-lorraine.fr).  