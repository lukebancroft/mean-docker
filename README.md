# mean-docker
mean-docker est un Docker Compose d'une MEAN stack contenant trois contenaires :
- La première contient l'application Angular en elle-même, cette application permet de faire des opérations CRUD sur une liste d'employés
- La seconde contient le serveur Express, elle permet de faire le lien entre l'application et la base de données
- La dernière est basée sur l'image docker officielle de MongoDB, c'est là que sont stockés les données

La partie applicative de cette application est basée sur le repository suivant :
https://github.com/CodAffection/MEAN-Stack-CRUD-Operations

---
Installation
-

- Assurez-vous d'avoir bien installé docker sur votre machine
- Télécharez ensuite les sauvegardes des 3 images docker ici : 
- Chargez les images sur votre machine une par une à l'aide de la commande :
```sh
docker load -i /chemin/vers/image/monimage.tar
```
- Utilisant le fichier docker-compose.yml, éxectuez la commande suivante :
```sh
docker-compose up
```
- Vous pouvez désormais utiliser l'application sur http://localhost:5555/, vous pourrez également vérifier le fonctionnement du serveur Express sur http://localhost:3000/ et MongoDB sur http://localhost:27017/

---

Projet M2 MBDS Nice Sophia Antipolis - Promo 2018/2019 - Enseignant: Gaëtan Robert Lescouflair - Docker
