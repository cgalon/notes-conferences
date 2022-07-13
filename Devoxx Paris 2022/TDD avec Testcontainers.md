---
conference: Devoxx FR
title: TDD avec Testcontainers
speaker: Julien Durillon
date: 2022-04-21
video: https://www.youtube.com/watch?v=-q7hLU2e2h4&list=PLTbQvx84FrARTeUA5pExVR5vjCOqWIplI&index=141
---
tags: #tests , #Testcontainers 

Pulsar : plateforme de messaging

But : pouvoir lancer les tests d'intégration en local

Lib Java qui s'intègre à JUnit et qui pilote du Docker

Directives @Testcontainers et @Container

Csa d'usages :
- Requêtes SQL
- Communication entre les services
- Non regression
- APIs

Utilise des images de base.
Fournit des classes de manipulation des images de base
Possibilité d'utiliser une classe générique pour les images non supportées

