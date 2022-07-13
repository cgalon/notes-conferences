---
conference: Devoxx FR
title: Tekton, nouvelle approche pour les pipelines
speaker: Philippe Thomas
date: 2021-09-29
video: https://www.youtube.com/watch?v=ENMAs_KG2lI&list=PLTbQvx84FrATKYTSVVei8ZouXFGePwSUA&index=26
---
tags: #cicd , #Kubernetes 

Open source : https://cd.foundation/

Tekton friends --> outils autour de Tekton (CLI, dashboard, catalog, hub)

Possibilité (future) de composer des pipelines avec d'autres pipelines

Cinq concepts :
- Step  (comme Concourse)
- Task  (comme Concourse)
- Pipeline  (comme Concourse)
- Trigger  (comme les resources Concourse)
- Catalog

Chaque step s'exécute dans un conteneur

Les tasks s'exécutent dans des pods

Hub et catalogues internalisables

Utilise des PVC pour passer les données entre les steps

Kubernetes native
