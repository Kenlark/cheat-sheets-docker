# Cheat Sheets Docker

Ce dépôt regroupe des fiches pratiques (cheat sheets) pour comprendre, installer et utiliser Docker, ainsi que des comparaisons avec d'autres technologies de virtualisation.  
Il s'adresse aux débutants comme aux utilisateurs souhaitant réviser rapidement les concepts essentiels autour de Docker.

## Table des matières

### 1. Introduction

- [Qu'est-ce qu'un Bare Metal ?](1.%20Introduction/bare-metal.md)
- [Comparaison entre un système Bare Metal, une machine virtuelle et Docker](1.%20Introduction/comparaison.md)
- [Qu'est-ce qu'un container ?](1.%20Introduction/container.md)
- [Qu'est-ce qu'une virtual machine ?](1.%20Introduction/virtual-machine.md)

### 2. Docker

- [Introduction à Docker](2.%20Docker/1.%20introduction-docker.md)
- [Différences entre images et conteneurs](2.%20Docker/2.%20difference-images-container.md)
- [Registre Docker](2.%20Docker/3.%20registre-docker.md)
- [Docker Hub](2.%20Docker/4.%20docker-hub.md)

### 3. Installation

- [Installation de Docker (Ubuntu/Debian)](3.%20Installation/installation-docker.md)

### 4. Commandes diverses

- [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)

### 5. Dockerfile

- [Introduction au Dockerfile](5.%20Dockerfile/1.%20intro-Dockerfile.md)
- [Construction d'une image Docker personnalisée](5.%20Dockerfile/2.%20construction-dune-image-docker-perso.md)
- [Push une image dans son repo Docker Hub](5.%20Dockerfile/3.%20commandes-docker-hub.md)
- [Le cache dans un Dockerfile](5.%20Dockerfile/4.%20cache.md)
- [Le Multi-stage Build dans Docker](5.%20Dockerfile/5.%20multi-stage-build.md)

### 6. Stockage dans Docker

- [Introduction au stockage dans Docker](6.%20Stockage-Dans-Docker/1.%20introduction.md)
- [Les volumes Docker](6.%20Stockage-Dans-Docker/2.%20volumes-docker.md)
- [Les bind mounts](6.%20Stockage-Dans-Docker/3.%20bind-mounts.md)
- [Les tmpfs mounts](6.%20Stockage-Dans-Docker/4.%20tmpfs-mount.md)
- [Stockage et sécurité dans Docker](6.%20Stockage-Dans-Docker/5.%20stockage.md)

### 7. Réseautage

- [Introduction au réseautage Docker](7.%20Réseautage/1.%20introduction.md)
- [Création et gestion des réseaux](7.%20Réseautage/2.%20creation-gestion-reseaux.md)
- [Connexion des conteneurs](7.%20Réseautage/3.%20connexion-conteneurs.md)

### 8. Docker-Compose

- [Introduction à Docker Compose](8.%20Docker-Compose/1.%20introduction.md)
- [Commandes Docker Compose](8.%20Docker-Compose/2.%20commands-docker-compose.md)

## Tableau récapitulatif des commandes Docker

| Commande                                                                                        | Description                                                    | Lien vers la fiche                                                                        |
| ----------------------------------------------------------------------------------------------- | -------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `docker pull <image>`                                                                           | Télécharger une image depuis un registre                       | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker run ...`                                                                                | Lancer un conteneur                                            | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker run --name <nom> -p 8080:80 -d <image>`                                                 | Lancer un conteneur avec port exposé                           | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker run -it ubuntu bash`                                                                    | Lancer un conteneur Ubuntu en mode interactif                  | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker run <image> echo "Hello world"`                                                         | Exécuter une commande non-interactive                          | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker create <image>`                                                                         | Créer un conteneur sans le démarrer                            | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker start <nom>`                                                                            | Démarrer un conteneur existant                                 | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker stop <nom>`                                                                             | Arrêter un conteneur                                           | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker restart <nom>`                                                                          | Redémarrer un conteneur                                        | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker rm <nom>`                                                                               | Supprimer un conteneur                                         | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker rm -f <nom>`                                                                            | Forcer la suppression d'un conteneur                           | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker rmi <image>`                                                                            | Supprimer une image                                            | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker rmi -f <image>`                                                                         | Forcer la suppression d'une image                              | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker ps`                                                                                     | Lister les conteneurs actifs                                   | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker ps -a`                                                                                  | Lister tous les conteneurs                                     | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker logs <nom>`                                                                             | Voir les logs d'un conteneur                                   | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker stats <nom>`                                                                            | Voir l'utilisation des ressources                              | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker inspect <nom>`                                                                          | Voir les informations détaillées d'un conteneur                | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker build -t <image> .`                                                                     | Construire une image à partir d'un Dockerfile                  | [Construction image Docker](5.%20Dockerfile/2.%20construction-dune-image-docker-perso.md) |
| `docker images`                                                                                 | Lister les images locales                                      | [Introduction Dockerfile](5.%20Dockerfile/1.%20intro-Dockerfile.md)                       |
| `docker tag <image>:<tag> <utilisateur>/<repo>:<tag>`                                           | Taguer une image pour Docker Hub                               | [Commandes Docker Hub](5.%20Dockerfile/3.%20commandes-docker-hub.md)                      |
| `docker push <utilisateur>/<repo>:<tag>`                                                        | Pousser une image sur Docker Hub                               | [Commandes Docker Hub](5.%20Dockerfile/3.%20commandes-docker-hub.md)                      |
| `docker login`                                                                                  | Se connecter à Docker Hub                                      | [Commandes Docker Hub](5.%20Dockerfile/3.%20commandes-docker-hub.md)                      |
| `docker run --name <nom> -d <utilisateur>/<repo>:<tag>`                                         | Lancer un conteneur depuis une image Docker Hub                | [Commandes Docker Hub](5.%20Dockerfile/3.%20commandes-docker-hub.md)                      |
| `docker volume create <nom>`                                                                    | Créer un volume Docker                                         | [Les volumes Docker](6.%20Stockage-Dans-Docker/2.%20volumes-docker.md)                    |
| `docker volume ls`                                                                              | Lister les volumes                                             | [Les volumes Docker](6.%20Stockage-Dans-Docker/2.%20volumes-docker.md)                    |
| `docker volume inspect <nom>`                                                                   | Inspecter un volume                                            | [Les volumes Docker](6.%20Stockage-Dans-Docker/2.%20volumes-docker.md)                    |
| `docker volume rm <nom>`                                                                        | Supprimer un volume                                            | [Les volumes Docker](6.%20Stockage-Dans-Docker/2.%20volumes-docker.md)                    |
| `docker volume prune`                                                                           | Supprimer les volumes orphelins                                | [Les volumes Docker](6.%20Stockage-Dans-Docker/2.%20volumes-docker.md)                    |
| `docker run -d -v <volume>:/data <image>`                                                       | Monter un volume dans un conteneur                             | [Les volumes Docker](6.%20Stockage-Dans-Docker/2.%20volumes-docker.md)                    |
| `docker run -d -v ${pwd}:/app <image>`                                                          | Bind mount pour développement                                  | [Les bind mounts](6.%20Stockage-Dans-Docker/3.%20bind-mounts.md)                          |
| `docker run -d -v /chemin/sur/hote:/chemin/dans/conteneur <image>`                              | Bind mount détaillé                                            | [Les bind mounts](6.%20Stockage-Dans-Docker/3.%20bind-mounts.md)                          |
| `docker run -d --mount type=bind,source=/chemin/sur/hote,target=/chemin/dans/conteneur <image>` | Bind mount syntaxe --mount                                     | [Les bind mounts](6.%20Stockage-Dans-Docker/3.%20bind-mounts.md)                          |
| `docker run -d --env-file <fichier.env> -v <volume>:/chemin <image>`                            | Exemple volume + env-file                                      | [Les volumes Docker](6.%20Stockage-Dans-Docker/2.%20volumes-docker.md)                    |
| `docker run --tmpfs /app/temp:rw,size=100m <image>`                                             | Utiliser un tmpfs mount                                        | [Les tmpfs mounts](6.%20Stockage-Dans-Docker/4.%20tmpfs-mount.md)                         |
| `docker exec -it <nom> bash`                                                                    | Ouvrir un terminal dans un conteneur                           | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `docker rename <ancien> <nouveau>`                                                              | Renommer un conteneur                                          | [Commandes Docker courantes](4.%20Commandes%20diverses/commandes-docker.md)               |
| `du -sh <chemin_du_volume>`                                                                     | Vérifier la taille d'un volume (commande système)              | [Les volumes Docker](6.%20Stockage-Dans-Docker/2.%20volumes-docker.md)                    |
| `mkdir /path/to/secure_data`<br>`chmod 700 /path/to/secure_data`                                | Sécuriser un dossier sur l'hôte (commandes système)            | [Stockage et sécurité](6.%20Stockage-Dans-Docker/5.%20stockage.md)                        |
| `docker network create --driver bridge <nom_reseau>`                                            | Créer un réseau Docker bridge                                  | [Création et gestion des réseaux](7.%20Réseautage/2.%20creation-gestion-reseaux.md)       |
| `docker network ls`                                                                             | Lister les réseaux Docker                                      | [Création et gestion des réseaux](7.%20Réseautage/2.%20creation-gestion-reseaux.md)       |
| `docker run -d --name <nom> --network <nom_reseau> <image>`                                     | Lancer un conteneur connecté à un réseau                       | [Création et gestion des réseaux](7.%20Réseautage/2.%20creation-gestion-reseaux.md)       |
| `docker network rm <nom_reseau>`                                                                | Supprimer un réseau Docker                                     | [Création et gestion des réseaux](7.%20Réseautage/2.%20creation-gestion-reseaux.md)       |
| `docker network connect <nom_reseau> <nom_conteneur>`                                           | Connecter un conteneur existant à un réseau                    | [Connexion des conteneurs](7.%20Réseautage/3.%20connexion-conteneurs.md)                  |
| `docker-compose up`                                                                             | Démarrer tous les services définis                             | [Commandes Docker Compose](8.%20Docker-Compose/2.%20commands-docker-compose.md)           |
| `docker-compose up -d`                                                                          | Démarrer tous les services en arrière-plan                     | [Commandes Docker Compose](8.%20Docker-Compose/2.%20commands-docker-compose.md)           |
| `docker-compose stop`                                                                           | Arrêter les services sans les supprimer                        | [Commandes Docker Compose](8.%20Docker-Compose/2.%20commands-docker-compose.md)           |
| `docker-compose down`                                                                           | Arrêter et supprimer les conteneurs, réseaux, volumes anonymes | [Commandes Docker Compose](8.%20Docker-Compose/2.%20commands-docker-compose.md)           |
| `docker-compose restart [service_name]`                                                         | Redémarrer tous les services ou un service spécifique          | [Commandes Docker Compose](8.%20Docker-Compose/2.%20commands-docker-compose.md)           |
| `docker-compose logs`                                                                           | Voir les logs de tous les services                             | [Commandes Docker Compose](8.%20Docker-Compose/2.%20commands-docker-compose.md)           |
| `docker-compose logs -f`                                                                        | Voir les logs en temps réel                                    | [Commandes Docker Compose](8.%20Docker-Compose/2.%20commands-docker-compose.md)           |

## Structure du dépôt

- **1. Introduction/** : Concepts de base (bare metal, VM, conteneur, comparaisons).
- **2. Docker/** : Explications sur Docker, images, conteneurs, registres, Docker Hub.
- **3. Installation/** : Guide d'installation de Docker sur Ubuntu/Debian.
- **4. Commandes diverses/** : Commandes Docker essentielles et astuces.
- **5. Dockerfile/** : Tout sur les Dockerfiles, de l'intro aux techniques avancées.
- **6. Stockage-Dans-Docker/** : Volumes, bind mounts, tmpfs, sécurité et bonnes pratiques.
- **7. Réseautage/** : Concepts et commandes pour la gestion des réseaux Docker, création, gestion et connexion des conteneurs en réseau.
- **8. Docker-Compose/** : Introduction et commandes pour l'orchestration multi-conteneurs avec Docker Compose.
