🐳 # Publie ton Image sur Docker Hub

 Tu vois l'image que tu as faite dans l'exo 2 ?  Maintenant, il faut la publier sur le hub, et je ne veux pas entendre : 'Monsieur, je n'y arrive pas.' Ça prend trois minutes sur Google pour trouver la réponse.

# Reponse

1. run 
```bash
docker login -u adrienduc
```

2. run 
```bash
docker tag exo2:v1 adrienduc/exo2:v1
```

3. run 
```bash
docker push adrienduc/exo2:v1
```