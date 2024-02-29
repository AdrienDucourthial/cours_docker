Oh oh problémo 😕: tu as une application node qui utilise un contenaire de base de données PostgreSQL vue précédemment, comment tu vas les faire communiquer ? 

Sachant qu'un contenaire est isolé... 🤔 Débrouille-toi !

L'application devrait renvoyer les noms dans la table "personnes".

# REPONSE

1. creer un network docker 
```bash
docker network create exo6-multi
```

2. modifier server.js pour lier les deux images et ecrire le Dockerfile de l'exo6.

3. lancer les deux images sur le network
```bash
docker run -d --network exo6-multi --network-alias postgres exo5:v1
docker run -d --network exo6-multi -p 3000:3000 exo6:v1
```

3. verifier sur navigateur qu'on a recuperer la liste des personnes