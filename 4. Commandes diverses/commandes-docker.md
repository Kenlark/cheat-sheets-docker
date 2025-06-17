# Commandes Docker

# Télécharger une image Docker depuis Docker Hub

```zsh
docker pull <nom_image>
```

# Créer un conteneur (sans le démarrer)

```zsh
docker create <nom_image>
```

# Démarrer un conteneur avec un port exposé

```zsh
docker run --name <nom_du_conteneur> -p 8080:80 -d <nom_de_l'image>
```

**Accéder à l’application : http://localhost:8080**

# Démarrer un conteneur existant

```zsh
docker start <nom_du_conteneur>
```

# Redémarrer un conteneur

```zsh
docker restart <nom_du_conteneur>
```

# Arrêter un conteneur

```zsh
docker stop <nom_du_conteneur>
```

# Supprimer un conteneur

```zsh
docker rm <nom_du_conteneur>
```

# Supprimer une image

```zsh
docker rmi <nom_image>
```

# Forcer la suppression d’un conteneur et/ou image

```zsh
docker rm -f <nom_du_conteneur>
docker rmi -f <nom_image>
```

# Lister les conteneurs actifs

```zsh
docker ps
```

# Lister tous les conteneurs (y compris arrêtés)

```zsh
docker ps -a
```

# Voir les logs d’un conteneur

```zsh
docker logs <nom_du_conteneur>
```

# Voir l’utilisation des ressources (CPU, RAM, etc.)

```zsh
docker stats <nom_du_conteneur>
```

# Voir les informations détaillées d’un conteneur

```zsh
docker inspect <nom_du_conteneur>
```

# Construire une image à partir d’un Dockerfile

```zsh
docker build -t <nom_de_l’image> .
```

# Exécuter une commande dans un conteneur (mode interactif)

```zsh
docker exec -it <nom_du_conteneur> bash
```

# Exécuter une commande dans un conteneur (non-interactif)

```zsh
docker run <nom_image> echo "Hello world"
```

# Renommer un conteneur

```zsh
docker rename <ancien_nom> <nouveau_nom>
```
