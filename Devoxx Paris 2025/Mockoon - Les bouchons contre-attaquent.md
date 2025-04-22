---
conference: Devoxx FR
title: Mockoon - Les bouchons contre-attaquent
speaker: Ivan Béthus
date: 2025-04-17
video:
---
tags: #bouchons, #tests 

Mockoon dispo en CLI et GUI

Possible d'importer le swagger d'une API

Peut utiliser Faker pour générer de la fausse donnée

On lance le serveur Mockoon pour générer de la donnée à la volée

Permet de gérer des bouchons "statefulls" (donnée persistante entre les requêtes)

Peut être utilisé en mode proxy pour les API dont on a pas la définition
-> Permet de créer les mocks à partir des logs des services appelés

Déploiement : 
- Package npm
- Image Docker
- Github Action

La CLI permet de générer un Dockerfile

Plus rapide à mettre en place que Wiremock
Moins de fonctionnalités que Wiremock

Opensource
Doc bien faite



