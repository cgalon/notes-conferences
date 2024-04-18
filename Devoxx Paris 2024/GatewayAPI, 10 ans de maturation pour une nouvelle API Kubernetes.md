---
conference: Devoxx FR
title: GatewayAPI, 10 ans de maturation pour une nouvelle API Kubernetes
speaker: Kevin Davin
date: 2024-04-18
video:
---
tags: #Kubernetes 

Ingress problématique dans Kube

En 2019 création de la spec pour une Gateway API.
- Role oriented
	- Network engineer
	- Cluster operator
	- Platform engineer
	- ...
- Compatible depuis les versions 1.24

La GatewayClass est une implémentation de la Gateway

Les devs écrivent des Route attachées aux Gateway qui sont instanciées par des GAtewayClass.

Possibilité de faire du mirroring (en fire and forget) pour tester 2 versions d'appli à la fois.
On peut aussi faire du blue-green avec une répartition du trafic en pourcentage entre 2 versions

Beaucoup d'implémentations disponibles

Projet ingress2gateway en cours de dev pour migrer un grand nombre d'ingress (mais vérifier le résultat)


