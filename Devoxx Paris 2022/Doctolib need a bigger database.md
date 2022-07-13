---
conference: Devoxx FR
title: Doctolib need a bigger database
speaker: David Gageot
date: 2022-04-22
video: https://www.youtube.com/watch?v=1PtPVpFWtKQ&list=PLTbQvx84FrARTeUA5pExVR5vjCOqWIplI&index=143
---
tags: #DB 

1 seule grosse DB : PostgreSQL sur AWS Aurora

AWS Aurora :
- 100% PostgreSQL
- Auto scaling (8 minutes pour démarrer une nouvelle instance)

Travail sur la couche applicative pour accélérer et fluidifier les devs (et cacher lespb techniques)

Load tests avec 2x la prod pour voir à quelle distance est le mur.

Plusieurs candidats pour changer de base :
- Spanner
- Yugabyte
- Citus MX
- Vitess

Spanner
- Stockage distribué
- Uniquement Google Cloud

Citus MX
- Extension au dessus de PostgreSQL
- MX : Permet de distribuer directement de traffic sur les workers

Yugabyte
- Pas d'autoscaling
- Encore jeune

Pas de choix fait
Stratégie de splitter la base







