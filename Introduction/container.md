# Qu'est-ce qu'un container ?

Un container est une unité légère, portable et isolée qui permet d'exécuter une application avec toutes ses dépendances dans un environnement cohérent, sans avoir à installer l'application directement sur l'hôte.

C'est une alternative plus légère et plus rapide aux machines virtuelles.

## Description

Un container est un environnement isolé qui contient tout ce dont une application a besoin pour fonctionner (code, bibliothèques, fichiers de configuration), et qui tourne sur le noyau du système d'exploitation de l'hôte, sans embarquer son propre OS complet.

## Structure

**[ Matériel physique ]**  
**[ OS de l'hôte (ex : Linux) ]**  
**[ Docker Engine (ou Podman, etc.) ]**  
    → **[ Container 1 : app + dépendances ]**  
    → **[ Container 2 : app + dépendances ]**


**Contrairement à une VM :**

- Le container ne contient pas un OS complet.

- Il partage le noyau du système de l’hôte.

- Il est beaucoup plus léger et démarre en quelques millisecondes.
