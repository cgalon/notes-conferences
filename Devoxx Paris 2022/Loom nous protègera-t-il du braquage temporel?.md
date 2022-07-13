---
conference: Devoxx FR
title: Loom nous protègera-t-il du braquage temporel?
speaker: José Paumard, Rémi Forax
date: 2022-04-20
video: https://www.youtube.com/watch?v=wx7t69DylsI&list=PLTbQvx84FrARTeUA5pExVR5vjCOqWIplI&index=162
---
tags: #Java 

https://dev.java

Programmation concurrente

Ancètres : Classes Thread et Runnable

2011 :Fork et Join

Loom : Possibiilité de détacher un threa de sa tache.
--> Threads virtuels
--> N'utilisent pas la pile de 2Mo d'un trhead classique

Quand le thread virtuel est bloqué, on "sort"le thread virtuel du thread de l'OS et on en met un autre

2 builders dans Thread : 
- 1 pour les threads virtuels
- 1 pour les threads platform

Si la pile du thread virtuel contient du C il se comporte comme un thread plateforme. (Parce que le C utilise des adresses physiques pour les pointeurs et que les piles ne sont pas toujours recopiées au même endroit)

Structured Concurrency
--> module jdk.incubator.concurrent




