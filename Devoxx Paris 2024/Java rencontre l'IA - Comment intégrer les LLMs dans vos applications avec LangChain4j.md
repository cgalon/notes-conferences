---
conference: Devoxx FR
title: "Java rencontre l'IA : Comment intégrer les LLMs dans vos applications avec LangChain4j"
speaker: Lize Raes
date: 2024-04-18
video:
---
tags: #ia 

Composants de LangChain4J : 
---Photo---

Repo Github : langchain4j/langchain4j
-> Bonne doc
-> Liste des intégrations avec les systèmes externes
-> Exemples

# Outils de base

AIServices permet de transformer du texte en POJO Java. (Dates, listes....)

Tools
On déclare des méthodes avec des annotations avec du texte descriptif et le LLM sait s'il doit utiliser les tools ou pas.

# RAG

## Naive RAG
Il existe plein de loaders différents

EmbeddingModel pour vectoriser dans un EmbeddingStore et un ContentRetriever pour la recherche.

## Advanced RAG
---Photo---
Utilise plusieurs objets pour implémenter et spécialiser le RAG.
Utilise des interfaces -> Permet de fournir ses propres implémentations.

Conseils de l'équipe : 
---Photo---

Repo exemples : langchain4j/langchain4j-examples






