---
conference: Devoxx FR
title: Oubliez Docker, appelez moi Compose
speaker: Nicolas de Loof
date: 2022-04-20
video: https://www.youtube.com/watch?v=xGh4F6_Gs0Y&list=PLTbQvx84FrARTeUA5pExVR5vjCOqWIplI&index=4
---
tags: #Docker 

fig (ancien orchestrateur) racheté par Docker --> docker-compose

Format des fichiers docker-compose compatible avec plusieurs solutions de cloud (swarn, aws...)

Format 2.x : compatibilité fig
Format 3.x : plutôt destiné au cloud

Création d'une spec pour compose : compose specification
- suppression de la version dans le fichier
- renommage du fichier en compose.yml
- compose intégré à la CLI docker
- fichier compose uniquement utile pour créer les ressources, pour le reste du cycle de vie, on gère avec les ressources nommées
- ajout des secrets



