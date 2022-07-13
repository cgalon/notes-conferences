---
conference: Devoxx FR
title: Déployer son application avec Argo dans Kubernetes
speaker: Paul Henry Perrissel, Nicolas Mpacko Tongo
date: 2022-04-21
video: https://www.youtube.com/watch?v=9B3VppgPsYk&list=PLTbQvx84FrARTeUA5pExVR5vjCOqWIplI&index=37
---
tags: #Argo , #Kubernetes , #cicd 

Boite à outil :
- Argo Workflow : 
- Argo CD
- Argo Rollout
- Argo Event

# Argo workflow

Crée des objets K8S

Peut orchestrer des jobs en parallèle

Ressemble aux pipelines Concourse

Script : pour faire du post ou pre processing pour une tache

Plus de types d'actions qu'avec Concourse

Beaucoup d'objet différents

Permet de scheduler des jobs

Interface assez évoluée

# Argo CD

Plateforme de déploiement sur K8S
Gère des états dans K8S

Interface visuelle des déploiements sur les clusters

Possible de configurer les outils de déploiement

Crée de nouveaux objets K8S

L'IHM peut se synchroniser avec le cluster



