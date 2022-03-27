# ZZ Book

Application microservice pour le cours de Technologie des conteneurs.

## Code des services

Le code des différents services est présent dans `src/`.

* `details` : Service de détails des livres, en ruby.
* `productpage` : Service point d'entrée des autres microservices, en python.
* `reviews` : Service contenant les commentaires sur les livres, appel `ratings`, en java.
* `ratings` : Service de gestion des notes des livres, en node.js.

## Définitions de l'API

L'API visible de l'utilisateur est définie dans le fichier `swagger.yaml`. Pour visualiser le fichier, vous pouvez utiliser le [Swagger editor](https://editor.swagger.io/).

## Registry

Le registry local est créé avec le script kind-with-registry.sh. 

## Réponses aux questions

Pour le TP3 les réponses sont dans le dossier TP3.
Pour le TP4, les réponses sont dans les commits.

## Groupe
Maxime Audigié - maxime.audigie@etu.uca.fr
Lucas Peyron - lucas.peyron@etu.uca.fr
