---
conference: Devoxx FR
title: Comment OpenTelemetry peut transformer votre monitoring
speaker: Vincent Behar
date: 2022-04-22
video: https://www.youtube.com/watch?v=dGMN3keJuXA&list=PLTbQvx84FrARTeUA5pExVR5vjCOqWIplI&index=125
---
tags: #Monitoring 

logs --> évènements bruts
Pb : standardisation

Même pb pour les métriques

Trace : timing d'une opération (plus autres infos)
--> Jaeger

Besoin de corrélation entre les 3 sujets

Exemple : partir d'un graphe Grafana sur des temps de réponses, on peut se débrancher sur les logs et les temps d'exec de chaque élément

Projet OpenTelemetry
- Des spécifications
- Des implémentations
- Un collecteur

#todo Insérer la photo de l'archi d'OpenTelemetry

Ajout d'idenitifiant "de corrélation" pour que le collecteur puisse agréger les données

#todo Insérer la photo de l'archi d'OpenTelemetry avec l'intérieur du collecteur






