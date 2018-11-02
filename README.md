# Cinema version statique #

Gérer la liste des films

Ce projet comporte un point d'entrée depuis le client:

**GET** `http://localhost:8080/affiche?id=n` qui renvoie l'image de
l'affiche du film dont l'identifiant est **n**

### Travaux pratiques

###### Créer une servlet qui affiche la liste des tritres de films
* La liste devra être triée par ordre alphabétique croissant,
* chaque titre est un lien vers le détail du film
* Paramétrer la servlet pour afficher les films par :
  - ordre alphabétique croissant/décroissant
  - note croissante/décroissante
  - par défaut c'est ordre alphabétique croissant



###### Créer une serlvet qui affiche le détail d'un film
* Titre
* Affiche
* Note

**GET** `http://localhost:8080/film?id=n` renvoie le détail du film dont
l'identifiant est **n**



###### Créer une servlet et son formulaire associé qui permettent de rechercher un film par titre

Faire en sorte que le critère de recherche ne soit pas sensible à la casse (aux majuscules et minuscules) et qu'il constitue une partie du résultat

Par exemple, la recherche du titre sur 'ju' pourra renvoyer des résultats comme 'Le juge et l'Assasin', 'La jurée', etc.


###### Gestion de la session utilisateur

Dans la session de l'utilisateur enregistrez l'ensemble des films dont il a
consulté le détail, l'utilisateur peut consulter son historique.

###### Gestion des ressources externes

Stocker les affiches dans un dossier de l'application n'est pas la
meilleure idée qui soit : si on peut ajouter des films et qu'on met
à jour l'application, toutes les affiches associées aux films seront
effacées. Paramétrer l'application pour que les affiches soient stockées
et récupérées dans un dossier externe et indépendant.