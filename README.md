**Nom    :** BUREAUX Axel, QUEVAL Martin, MARROUCHE Mohamad
**Groupe :** Groupe 2
**Année  :** 2023

# docker-sae203

Pour la SAE on a pas pu faire ce qu'on voulait qui était de pouvoir publier des vidéos sur le site et que d'autres utilisateurs pouvaient les voir. Pour la SAE 2.03 on devait créer une applcation statique avec une base de donnée locale. Pour satisfaire aux besoins demandées, nous avons crée un service de vidéos en ligne avec 3 différents comptes. Suite à ca, nous avons essayé de continuer notre idée originale. En utilisant docker-compose pour lancer le site et des images de mySQL et aussi PHPMyAdmin déjà conçu sur docker, nous avons pu créer le site. Notre projet marche parfaitement, on a essayé avec des camarades de la classe, ils ont pu ajouter des vidéos et on les voyait en même temps.

## Comment installer le site ?

1. Construire l'image via le Dockerfile (commande à exécuter dans le dossier où se trouve le dit Dockerfile)

       docker build -t <nom image> .

2. Créer un conteneur docker avec l'image créée plus tôt

       docker run -d -p <port>:80 <nom image>
       
3. Accéder au site en entrant dans la barre d'adresse :

       localhost:<port>


## Comment installer le site avec notre docker-compose?

1. Construire l'image via le docker-compose.yaml (commande à exécuter dans le dossier où se trouve le dit docker-compose.yaml)

       docker-compose up 
 
2.Accéder au site en entrant dans la barre d'adresse :

       localhost:9000
  
3.Accéder à PHPMyAdmin en entrant dans la barre d'adresse :

       localhost:8080
       
