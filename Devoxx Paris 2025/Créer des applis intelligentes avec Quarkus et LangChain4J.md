---
conference: Devoxx FR
title: Créer des applis intelligentes avec Quarkus et LangChain4J
speaker: Zineb Bendhiba, Clément Escoffier
date: 2025-04-16
video:
---
tags: #ia , #rag , #Quarkus 

Reasoning models
-> Raisonnement multi-steps

Quarkus LangChain4J

![[20250416_134415.jpg]]

-> Annotations spécifiques pour l'IA

Les limites du RAG : 
- Comment splitter les docs
- Overmatching
- Undermatching

Contextual RAG
-> Contextualiser la query (résumé par exemple)
-> Query router (identifier la bonne source documentaire)
-> Content Aggregator (Reranking)
-> Corrective RAG (on évalue le contenu du RAG et on recommence si besoin)

Function calling possible aussi avec Quarkus
-> Description des tools (@Tool)
-> Guardrails (programmation défensive sur les prompts)

![[20250416_140844.jpg]]

Model Context Protocol

![[20250416_141630.jpg]]




