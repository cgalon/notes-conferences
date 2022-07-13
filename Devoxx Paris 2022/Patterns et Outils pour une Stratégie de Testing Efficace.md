---
conference: Devoxx FR
title: Patterns et Outils pour une Stratégie de Testing Efficace
speaker: Younes Jaadi
date: 2022-04-12
video: Pas de vidéo. Session supplémentaire organisée par Oxiane.
---
tags: #Javascript , #tests 

Session organisée par Oxiane la semaine avant Devoxx.

# Pourquoi tester
Arrêter de tester manuellement à chaque changement
Sécurité quand on fait une modif
Boucle de feedback
Confiance
Améliore le collective ownership
Améliore les possibilités de refactoring
La meilleure doc ce sont les tests

**Les freins :**
- Le ticket d'entrée
	- Pair programming
	- Projet de carrière
- Le nombre de lignes de code produites
	- Biais de temps de développement
	- Beaucoup plus long de faire des tests manuels à répétition
	- Le cout des lignes produites sans test augmente avec le temps


# Les types de tests
Narrow tests vs Wide tests

## Narrow tests
Fast (<100ms)
Diag instantané
Isolation et parallélisation sans effort
On peut utiliser une BD en mémoire si ça va vite

## Wide tests
Plus lents
Plus difficile à diag
Plus de surface couverte

# Les stratégies de test
Stratégie en cornet de glace (pyramide inversée) --> Bof
NB : Mise en prod de code != activation en prod
Pyramide classique --> Risque de trop petits tests avec peu de sens
Stratégie en hexagone (honeycomb)

