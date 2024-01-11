# 🚀 Guide d'utilisation de l'image Docker

Cet exercice consiste à trouver un moyen de lancer l'image Docker disponible à l'adresse suivante : [docsseo91/stardocker sur Docker Hub](https://hub.docker.com/r/docsseo91/stardocker).


## 🏃 Comment lancer l'image Docker

Suivez ces étapes simples pour lancer l'image Docker :

1. Ouvrez votre terminal.

2. Utilisez la commande suivante pour télécharger l'image Docker depuis Docker Hub :
   ```bash
   docker  ...
   ```
Oups, j'ai failli donner la réponse. Allez, go !

# Reponse 

1. pull l'image
```bash
docker pull docsseo91/stardocker:v1
```

2. lancer l'image
```bash
docker run -d --platform linux/arm64 docsseo91/stardocker:v1
```