---
conference: Devoxx FR
title: Gérer la dette d'architecture dans un contexte d'hypercroissance
speaker: Cyril Beslay
date: 2023-04-13
video: https://youtu.be/F30CJnmzI8Y
---
tags: #dette

Dans un composant ou tout process fonctionnel c'est l'écart entre les systèmes actuels et les standards ou les précos de l'entreprise.

Exemples : 
- Non mise en place de Circuit breakers
- Mauvais choix de framework
- Changements de standards
- Utiliser directement la base d'une autre appli

Le business est la principale source de création de dette

Mêmes conséquences que pour la dette technique

Deux solutions : 
- Contrôler la création de la dette
- Réduire la dette existante

Penser l'architecture / Faire de la conception
Anticiper les besoins fonctionnels
Faire des ADR
Créer des tickets de dette

Règle du boyscout
20 du temps du sprint consacré à la dette
Investir plus de temps dans les refactos
Correction opportuniste
Gel des nouvelles fonctionnalités
Réécrire en entier un composant

Stratégie passive -> Délaisser jusqu'à ce que le composant meurre.

Plus simple de tout jeter et refaire mais moins instructif

Création d'un outil interne pour analyser le respect des règles. Affichage de la dette des équipes.

Tech radar spécifique à l'entreprise

Entretiens tous les trimestres avec les tech leads et les managers.
Questionnaire
Pour chaque building block --> score card : 
- Risk
- Time
- Impact
- Efficiancy
- Deviation

Cartographie par composant/equipe/domaine

Mettre en corrélation avec d'autres métriques
- Nombres d'anos
- ...

Si la dette est trop élevée, on suspend le dev des nouvelles fonctionnalités






