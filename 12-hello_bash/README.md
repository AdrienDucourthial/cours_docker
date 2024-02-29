Nous avons un stagiaire qui a utilisé **`chatgtp`** pour créer le `Dockerfile`, mais malheureusement, cela ne fonctionne pas correctement et il est incapable de nous expliquer ce que le `Dockerfile` est censé faire. Voici donc ta mission : 

1. **Réviser le `Dockerfile`** : Assure-toi qu'il soit bien écrit et qu'il fonctionne comme prévu. Rectifie toute erreur que tu pourrais trouver. 

2. **Tester le déploiement** : Après avoir corrigé le `Dockerfile`, teste 

3. **Documenter le processus** : Rédige une explication claire de ce que chaque ligne du `Dockerfile` fait et comment cela contribue au fonctionnement global du projet.


## 📝 Rendu Attendu
un Dockerfile fonctionnel, accompagné d'un README. Ce README devra inclure une explication détaillée du projet. 


## Explications 

Le fichier index.sh sert a créer un fichier index.html. J'ai créé le fichier index.html direct et je le copie direct au bon endroit.

*line 1* : FROM nginx:alpine

Ça sert a utiliser l'image nginx

*line 2* : COPY index.html /usr/share/nginx/html/index.html

Je copie le fichier index.html au bon endroit sur le docker pour que le site web soit correctement exposé.
Comme on ne modifie pas la conf nginx sur l'image, on est obligé de mettre le fichier index.html dans /usr/share/nginx/html/.