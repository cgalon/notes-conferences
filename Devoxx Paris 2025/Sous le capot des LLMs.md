---
conference: Devoxx FR
title: Sous le capot des LLMs
speaker: Guillaume Laforge, Didier Girard
date: 2025-04-16
video:
---
tags: #ia 

4 tokens <> 3 mots
1 token est un peu comme un emoji pour un LLM
Tokens plus efficaces pour faires des liens entre les parties d'une phrase

On peut fine tuner des modèles pour réduire le nombre de tokens (surtout sur les acronymes spécifiques à se boite) 

poloclub.github.io/transformer-explainer/
-> Pour comprendre comment fonctionne les LLMs

top-K : On ne prend que les x premiers tokens possblies
top-P : On utilise potentiellement que des tokens dont l'addition est dans une certaine valeurs  
Temperature : On ajoute du poids au premier token suivant possible

top-K = 1 et temp = 0 -> presque déterministe

Le contexte posé dans la question influence la réponse

Les LLMs connaissent les mots pas les concepts derrière (par exemple "hier")

Le Base64 est un langage comme un autre pour un LLM


