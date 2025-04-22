---
conference: Devoxx FR
title: Quand Java rencontre l'IA - Construisez des application AI en Java
speaker: Clément Escoffier, Emmanuel Bernard
date: 2025-04-17
video:
---
tags: #ia , #Java , #Quarkus 

Langchain4J diverge de Langchain maintenant

Surcouche Quarkuz à Langchain4j -> opinionated
Offre des abstractions pour des cas d'usages classiques
- Dialogue
- RAG
- function calling
- MCP
- ...

Dans les points d'intégration avec le modèle, Quarkus ajoute des services de manière transparente : 
- Observabilité
- Fault tolerance
- ...

![[20250417_142455.jpg]]

Les QueryRouter permettent de choisir entre plusieurs sources de documents.

Annotations @ToolBox et @Tool pour marquer et injecter les outils à utiliser
Utilise la description dans les annotations pour connaitre ce que fait l'outil

Possibilité d'utiliser des Guardrails pour sécuriser une architecture agentique

Standardise les interactions entre les éléments du RAG (MCP client, MCP server, LLM)
-> Plusieurs protocoles de transport
S'implémente en une annotation
Spécification de l'outil dans la conf

Nécessite des reasoning models

Activateur d'écosystème
Beaucoup de potentiel

Tests
3 modes de testing

![[20250417_162051.jpg]]

Librairie d'assertion fournie avec l'intégration de Quarkus
Demande au juge de vérifier certains critères de la réponse

Evaluation framework

![[20250417_163108.jpg]]







