---
conference: Devoxx FR
title: Simplifier l'usage des LLM dans le code avec Semantic Kernel
speaker: Eric Grenon, Louis Guillaume Morand
date: 2025-04-16
video:
---
tags: #ia , #rag 

Multitude de modèles potentiels à utiliser
Nouveaux usages des applications liés aux LLMs
Besoin d'orchestration entre les appels LLM et les appels API fonctionnels

Semantic Kernel : Middelware d'orchestration
- Plugins (RAG, function calling...)
- Planners : planifier une séquence d'actions
- Personas
- Memory : Gestion des dialogues, données contextuelles à la conversation

Config des tools en JSON

Implémente le function calling

Gère aussi des agents
-> acteur qui utilise un ou plusieurs modèles pour effectuer une tâche de manière semi-autonome
"Programmation agentique"
Un agent est spécialisé dans une tâche
Le framework gère les interactions avec tous les agents de votre application
On peut définir la stratégie d'interaction entre les agents

