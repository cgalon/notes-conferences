---
conference: Devoxx FR
title: De Compose à Kubernetes, Same player shoot again
speaker: Nicolas de Loof et Guillaume Lours
date: 2024-04-18
video:
---
tags: #Kubernetes , #Docker 

Compose -> Utilisé en local pour tester une stack
K8S utilisé en prod

Pour traduire les compose file en manifest K8S
Kompose : Tout n'est traduit

Compose on Kubernetes -> Echec
Docker ECS "Cloud integration" -> Echec

Nouvel outil : Compose Bridge

En entrée : compose.yaml standard
En sortie : manifest K8S standard
Puis utilise un autre transformer pour gérer les spécificités
Crée une arborescence kustomize

Il existe un transformer "helm"
On peut définir ses propres transformers



