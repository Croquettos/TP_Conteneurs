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

## Questions

### TP1

Q2) docker pull alpine
docker images

Q3) docker run -it --rm alpine
docker ps -> le conteneur est éteint

Q4) docker run --detach --name mariadbtest --env MARIADB_USER=root --env MARIADB_PASSWORD=root --env MARIADB_ROOT_PASSWORD=root

Q5) docker exec -it mariadbtest /bin/bash

Q7) docker run --name my-site --env AUTHOR=you -p 8080:80 dockersamples/static-site

### TP3

Q3) kubectl get namespaces pour voir les namespaces
Kube-system est le namespace pour les objets créés par le système de Kubernetes.

Q5) kubectl port-forward pod <nom_du_pod> 8080:8080

Q6) Le nombre de pods augmente.

### TP4

Q2) NodePort, on accede a l'app avec l'ip du node (kubectl get nodes -o wide -> INTERNAL-IP) et le port du NodePort (kubectl get svc pour voir le port si on ne l'a pas spécifié dans le manifest)

## Groupe
Maxime Audigié - maxime.audigie@etu.uca.fr
Lucas Peyron - lucas.peyron@etu.uca.fr
