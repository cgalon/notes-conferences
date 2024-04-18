---
conference: Devoxx FR
title: Utiliser les IA génératives avec Java - Au dela des simples chatbots
speaker: Abdel Sghiouar et Cédrick Lunven
date: 2024-04-17
video:
---
tags: #ia , #OpenSource , #rag 

Conférenciers de chez Google et Cassandra (un peu de pub)
# Introduction

LLM basés sur l'archi Transformers
https://lifearchitect.ai/models -> benchmark sur les LLM
Uses cases :
- Langage (écriture, idéation, résumé...)
- Code (Completion, génération...)
- Speech (Speech to text, texte to speech...)
- Vision (manips d'images...)

---Photo---

Vertex.AI : Offre globale de Google pour faire de l'IA
API Google Java pour appeler Gemini (google-cloud-vertexai)
-> Juste une dépendance dans Maven

3 versions de Gemini : Nano, Pro, Ultra
Gemini 1.5 -> 1 million de tokens

Chat : https://gemini.google.com (gratuit)
Générer des clé : https://ai.google.dev (gratuit)
Exemples : https://ai.google.dev/examples (gratuit)

# Gemma

Modèle OS
Dispo sur HuggingFace
Gemma disponible en 2B ou 7B
Pour faire tourner un LLM en local : Ollama

Abstraction pour l'API model : ChatLanguageModel (implem : OllamaChatModel ou VertexAIChatModel)

LangChain4j : Propose des abstractions et les fournisseurs de modèles implémentent les connecteurs

SpringAI : La même chose dans l'écosystème Spring

# Prompt engineering

Avoir une bonne structure de prompt
---Photo---
Toujours poser comme contrainte "Si tu ne sais pas dis que tu ne sais pas"

Tuner les paramètres
---Photo---

Technique avancée : 
- Chains of Thoughts (Chaine de pensée)
	-> Pour permettre aux LLM de raisonner
- Chain of Thoughts = self consistency
	-> Donner plusieurs solutions de raisonnement pour qu'il s'autovérifie
- ReAct (Reasoning and Acting)

Best practices
---Photo---
---Photo---

Prompt Templates in Java
-> Avec LangChain4J, SpringAI, GoodBards...
Classe : PromptTemplate

# Vector search

Le nombre de dimensions d'un vecteur dépend du modèle.
La norme, c'est la longueur d'un vecteur
Vector similarity :
- Distance euclidienne (Distance entre les "pointes" des vecteurs)
- Distance angulaire (cosine similarity)

Les formules de calcul peuvent différer selon les bases de données

Pour simplifier, les vecteurs générés sont de norme 1.
Peut faire sauter la précision des floats de Java.

Choix de la métrique : ---Photo---

HNSW : Hierarchical Navigable Small World

jVector : Moteur de recherche vectoriel en Java OS
Algo : DiskANN (Vamana + ??? + Oversampling)
10 fois plus rapide que Lucene

Plusieurs infos à stocker dans la base vectorielle : 
---Photo---

https://superlinked.com/vector-db-comparison

LangChain4J fournit un EmbeddingModel

Embedding Store : Langchain4j-xxx
Implementations de différents niveaux suivant les fournisseurs de l'implémentation

# RAG

(30 dernières minutes de la conf)

## Implémentation naive

Trop compliqué de vectoriser un document complet (perte d'infos sémantiques) -> Chunk
Plusieurs manières de chunker les documents
---Photo---

C'est OK de chunker en fonction d'un nombre de tokens fixes (en faisant attention à la fin des phrases)
Preprocessing du document pour le nettoyer.
Puis chunking de documents par nombre de tokens avec de l'overlaping entre les chunks
---Photo---

Quand on vérifie un RAG, il faut utiliser des docs persos pour que le LLM n'utilise pas ses propres connaissances.

## Implémentation avancée

Dans l'abtraction AIService de LangChain, on peut définir des QueryRouter pour spécialiser les recherches suivant le besoin.

On peut utiliser un QueryTransformer pour résumer les conversations trop longues, ou bien implémenter les règles de la boite.

On peut aussi travailler sur les réponses avec un QueryAggregator pour retravailler les réponses de la base (par exemple pour faire du reranking sur les réponses pour mieux les filtrer).
-> Meilleur en ce moment : Cohere

Plus de techniques avancées à explorer : 
---Photo---

## Function calling

Permet d'utiliser un service externe en fonction des questions (par exemple demander la météo actuelle d'un lieu)
-> Utilisation de Tools dans LangChain4J
-> Annotation de méthode spécifique et utilisation par LangChain en fonction de la sémantique de l'annotation

Sources : github datastaxdevs/conference-2à24-devoxx-france












