---
conference: Devoxx FR
title: Des tuyaux sur les pipelines
speaker: Philippe Charrière et Pierre-Antoine Grégoire 
date: 2023-04-12
video: https://youtu.be/1oRiEzMW6QA
---
tags: #pipeline , #cicd , #tests , #gitops , #bdd , #sécurité , #supervision , #observabilité 

Devops : 
- C : Culture
- A : Automatisation
- L : Lean
- M : Mesures
-  S : Sharing (Partage)

Dans Gitlab, on définit des stages (phases du pipeline)
Les jobs sont dans des stages.
Les stages s'excutent les uns après les autres
Les jobs sont en parallèle dans les stages
Si on utilise les MR, les rapports de qualimétrie ou de tests peuvent être consultés depuis l'IHM de Gitlab.

Pour avoir des messages de commit standards -> Git pre-commit hook

Un build doit pouvoir être exécuté en local ou sur la CI.
Paralléliser les tests trop lents
De temps en temps lancer un build sans cache pour vérifier que l'on en n'est pas dépendant.

Lancer les recherches de CVE au plus tôt.

Fuzz testing : fournit des données invalides, inattendues ou générées au hasard

Framework de micro-benchmarking : Hey, ab (apache benchmark)

Outils de sécurité : OWASP vulnerability scanning tools

SBOM -> Software Bill Of Material (Inventaire des composants logiciels utilisés)
Le SBOM peut être publié au moment du build
Format de SBOM : Owasp CycloneDX
Outil de génération de SBOM : Syft

Kaniko : Permet de builder des images Docker sans avoir besoin de démon Docker

Pour analyse et gestion des dépendances : DependaBot ou Renovate

GitOps : Git devient la source de vérité de ce qui doit être déployé.
-> Reproductibilité
-> Sécurisation

Démo avec FluxCD.
Déposer un agent de Flux dans K8S. Ensuite c'est l'agent qui va observer GitLab.
Flux créé un repo Gitlab
On fait la connexion entre la CI de Flux et le repo git

Le déploiement des données.
Modèle Expand/Contract :
- Phase 1 : Expand : Introduire le changement dans les structures existantes
- Phase 2 : Transition : Modif du code pour utiliser les nouvelles données.
- Phase d'attente : Pour que les nouvelles données se répandent
- Phase 3 : Contract : Supprimer les anciennes données qui ne sont plus utilisées
Outils : Flyway ou Liquibase pour introduire des changement de DB dans les pipelines

SAST : Analyse statique du code
DAST : Analyse dynamique du code
SCA : Analyse des dépendances
Les tests de sécu s'insérent dans le pipeline de déploiement
Ne doivent pas ralentir le pipeline
En cas d'erreur de sécurité, créer une issue avec un label dédié
Se faire aider par les équipes sécu le premier coup que l'on met en place les scans de sécu.

Monitorer les pipelines
MTTR....
Monitorer les tests
Monitorer les produits déployés

Mettre en place des canaris jobs : Pour vérifier que les briques nécessaires au pipeline sont bien là

Donner à voir la visibilité sur la sécu, la dispo des systèmes....
Donner de la visibilité sur les roadmaps...
Créer une base requêtable sur la base des SBOM



