# Commandes

## Pour télécharger une image docker depuis docker hub :

```zsh
docker create <nom_image>
```

## Pour lister tous les container :

```zsh
docker ps
```

**ou si les container sont arrêtés**

```zsh
docker ps -a
```

## Pour démarrer un conteneur d'une image :

```zsh
docker run --name <nom_de_votre_container> -p 8080:80 -d <nom_de_l'image>
```

**Vous pouvez vous connecter via localhost:8080 pour voir si votre conteneur fonctionne ou alors via `docker ps`**

## Pour voir les logs d'un conteneur :

```zsh
docker logs <nom_du_container>
```

## Pour voir les ressources d'un conteneur :

```zsh
docker stats <nom_du_container>
```

## Pour voir les informations détaillées d'un conteneur :

```zsh
docker inspect <nom_du_container>
```
