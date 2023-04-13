---
conference: Devoxx FR
title: CRAC vs GraalVM pour un démarrage rapide
speaker: Lilan Benoit
date: 2023-04-13
video: 
---
tags: #Crac , #GraalVM 

Changement de paradigme depuis les serveurs d'application

Usages de Java de plus en plus gourmands :
- Classloader
- Prise en compte des annotations (Entity, injection...)
- Blocs statiques
- Init des contextes applicatifs (CDI, Java...)

# GraalVM

- Compilateur Graal
- Native Image

Compilation complète en phase de construction

Solution d'Oracle Labs

Contraintes :
- Pas de dynamisme
- Pas de reflexion
- Utilisation de Substrate VM
- Serial GC (pas très performant)
- Optimisations à chaud et garbage G1 dans la version Enterprise

# CRAC

Coordinated Restore At Checkpoint

Solution d'OpenJDK
Se base sur la JVM

Checkpoint : Figer la JVM avec toutes les optimisations en cours
Commande pour indiquer où on stocke l'état de la JVM

Restore : Restoration de la JVM avec toutes les optim sauvegardées par le checkpoint
Commande pour indiquer quel checkpoint on récupère

Ajoute une lib accessible dans le code pour gérer les checkpoints et les restore.

Les checkpoints/restore ne gèrent pas les connexions :
- Besoin de fermer les connexions au moment du checkpoint.
- Besoin de recréer les connexions au restore.

Pris en compte par Springboot



