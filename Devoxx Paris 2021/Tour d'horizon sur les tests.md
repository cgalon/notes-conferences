---
conference: Devoxx FR
title: Tour d'horizon sur les tests
speaker: Yannick Grenzinger, Maxime Gellé
date: 2021-09-29
video: https://www.youtube.com/watch?v=AeuCcq_bCDw&t=48s
---
tags: #tests , #tdd , #bdd , #PropertyBasedTesting

Quatre niveaux pour une application : 
- Fragile
- Robuste
- Resilientt
- Anti Fragile

# Tests d'acceptance unitaires 

TDD

Utiliser des fakes à la place des mocks quand on peut

Sacraliser le métier 
- Archi hexagonale
- Arch unit

Mutation testing
- pitest.org

# BDD

Concept de Dan North --> **Spécification par l'exemple**
- 3 amigos
- Atelier : example mapping

Exprimer l'intention
Utiliser le langage métier
Cacher les détails techniques
Utiliser des persona
Expliciter le background
Un seul "when"
F.I.R.S.T.

CukeDoctor --> Produire des PDF à partir des rapports de test

Si le métier ne lit pas votre Gherkin, n'en écrivez pas.

Lectures : The BDD books : (Leanpub)
- Discovery
- Formulation
- Execution

Test d'intégration --> Tester justtes bouts techniques du composant

# Contract testing

- PACT
- Spring Clud Contract

```ad-tip
title: C'est le consommateur qui créé l'exemple
collapse: open
```

Outil Pact Broker --> Permet de vooqui utilise qui

# Tests UI

Long et compliqué
Deux solutions :
- Mocker le backend
- Tester juste quelques scénarios

Pattern Page Object
Screenplay pattern

# Tests exploratoires

Par les QA --> Expertise métier

# Property based testing

Outils : 
* jqiwk
* Quick Theories

# Testing in production

Pas possible de prévoir toutes les conditions d'échec en dehors de la prod
Article : Cindy Sridharan [Testing in production the safe way](https://copyconstruct.medium.com/testing-in-production-the-safe-way-18ca102d0ef1)

Chaos monkey --> Lib Netflix



