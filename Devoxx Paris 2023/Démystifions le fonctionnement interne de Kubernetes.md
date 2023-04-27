---
conference: Devoxx FR
title: Démystifions le fonctionnement interne de Kubernetes
speaker: Denis Germain
date: 2023-04-13
video: https://youtu.be/OCMNA0dSAzc
---
tags: #Kubernetes 

Plusieurs composants internes :
- API server -> Abstraction de l'infra
- etcd : base clé/valeur -> Stocke les objets K8S
- controller manager : écoute les évènements
- scheduler : positionne les pods où il faut
Ces 4 composants forment le control plane

- kubelet : agent
- container runtime : docker puis containerd

k8s utilise un réseau vituel -> utilise iptables ou ipvs

- CNI Plugin  : Pour créer le réseau virtuel, on a besoin d'une implémentation d'un CNI (container network interface) -> calico, flannel...

- IngressController (traefik, nginx...)

Au final c'est :
- un serveur d'API
- un ordonnanceur
- des boucles de controles
- un container runtime
- un réseau virtuel

