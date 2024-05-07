---
conference: Devoxx FR
title: La doc va bien, ne t'en fait pas.
speaker: Damien Lucas
date: 2024-04-17
video: https://youtu.be/zQ0A75HqFuA?si=TRbI-NtemCIFQd0Y
---
tags: #livingdoc 

Github : @dlucasd (Onepoint Bordeaux)

Arc42 : Template de documentation. Permet de décrire une architecture logicielle
Sources en asciidoc
Cf. Github de Arc42 (existe en français)
Propose une structure de doc (utilisée pour la conf)

# Introduction
Documentation d'API
-> Un standard : OpenApi
Outils :
- OpenApi generator (moins joli)
- ReDoc
- Swagger
Si pas de contrat d'interface :
- Springdoc
Si pas d'API Rest
- Asciidoclet

# Contraintes d'architecture

Visio
draw.io
C4 model
-> Vue 1 du modèle : Contexte

# Contexte

# Définition de la solution

Vue 2 du C4 : Conteneurs
Vue 3 du C4 : Composants
Vue 4 du C4 : Code

Fichier PlantUML pour créer ces modèles

Problème de PlantUML -> redondance des infos entre les vues

Structurizr -> Créé par le créateur de C4
DSL
Permet de définir le modèle as code
Utilise les vues de C4 pour structurer
Pas de redondance d'info: On définit les objets une seule fois et on les réutilise dans toutes les vues
Editeur en ligne -> Permet d'exporter les schémas dans différents formats

Autre solution : Compodoc (pour des applications Angular)
Dépendance Angular qui génère une doc complète à partir du code et de la jsdoc

# Vue exécution

Diag de séquence 
- Avec Mermaid par exemple (intégré à Github)

# Vue déploiement

Vue déploiement de C4 (avec Structurizr)
Avec K8S : k8sviz, KubeView
Docker compose : docker-compose-diagram, docker-compose-viz

# Concepts transversaux

Packaging, déploiement...
Pattern d'archi
Dépendances
Observabilité
Modèle de données
-> SchemaSpy : Pour représenter le modèle de données
	-> Reverse engineering de la base 
ADR (contexte, décision, statut)

# Critères de qualité

Détailler les critères de qualité avec des scénarios

# Risques et dettes techniques

# Glossaire

Termes techniques et métier importants
A partir d'annotations dans le code (@Glossaire)

# Divers

Outils pour générer de du Confluence à partir d'asciidoc

Diataxis : Pour la doc utilisateur
- Tutorials (Learning)
- How-to guides (Goals)
- Explanation (Understanding)
- Reference (Information)
Exemple doc de Quarkus

