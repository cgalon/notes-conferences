---
conference: Devoxx FR
title: Les métriques sont précieuses mais savoir quoi en faire l'est encore plus
speaker: Vincent Aubrun
date: 2025-04-18
video:
---
tags: #métriques, #observabilité , #alerting

Solution remote friendly

Etapes : 
- Fait la "carto" de la stack technique
- Définit les métriques à suivre par élément de la stack 
- Définit les seuils d'alerte pour chaque métriques
Puis
- Premier bilan de l'utilisation de ces métriques
- Actions d'ajustement sur les limites choisies
- Faire des tests de charge pour apprendre
- Bien définir les niveaux de logs
	- Revue des messages de log
	- Retirer les messages de logs inutiles

Alerting
- Définir les impacts de l’événement remonté par l'alerting
- Alerting sur des événements fonctionnels et pas seulement techniques
- Définition de seuils en fonction du moment de la journée
- Rations plus stables que les seuils
- Moins on a de valeurs plus les métriques sont erratiques
	- Monitorer en fonction du moment de la journée
- S'adapter à la réalité du système



