---
conference: Devoxx FR
title: Microservices et cohérence des données
speaker: JF James
date: 2022-04-22
video: https://www.youtube.com/watch?v=7HC6ZfSy8M4&list=PLTbQvx84FrARTeUA5pExVR5vjCOqWIplI&index=146
---
tags: #Java , #Microprofile 

Jusque là : transactions ACID

Monolithe modulaire : Transaction simple

Plusieurs modules avec plusieurs bases : 2 phases commit
Mais compliqué et super fiable

--> LRA/SAGA
Transactions ACID locales
En cas de pb, on passe des opérations locales de compensation

Les solutions :
- Microprofile (LRA)
- Enventuate (SAGA)
- AxonIQ
- SEATA

Bouquin : Microservices patterns

#todo : ajouter la photo du omparatif entre Microprofile et Eventuate



