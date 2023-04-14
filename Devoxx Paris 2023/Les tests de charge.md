---
conference: Devoxx FR
title: Les tests de charge
speaker: Stéphane Landelle
date: 2023-04-14
video: 
---
tags: #tests 

Permet de détecter des problèmes qui n'arrivent qu'avec de la charge

Ce n'est pas de la webperf. C'est coté serveur.
Génère du trafic réseau
Itératif. Corriger un pb après l'autre.

Se focaliser sur les fonctionnalités critiques

Ne pas tester les caches (changer les données entre les requêtes)

Comprendre le trafic réseau que l'on veut simuler

Choisir entre système ouvert ou fermé (avec une file d'attente)
Le système fermé permet de travailler en nombre d'utilisateurs concurrents

Déterminer le type de test que l'on veut (comportement d'arrivée des utilisateurs) :
- scale (montée progressive)
- stress (pic soudain)
- soak (sur la durée)
- smoke (1 seul utilisateur)

Ne pas mesurer la moyenne des temps de réponse
-> Utiliser des percentiles

Faire des tests régulièrement
Faire dans les équipes projet






