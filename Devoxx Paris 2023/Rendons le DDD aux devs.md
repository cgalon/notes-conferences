---
conference: Devoxx FR
title: Rendons le DDD aux devs!
speaker: Arnaud Thiefaine et Dorra Bartaguiz
date: 2023-04-12
video: https://youtu.be/3jI6TpzLU1c
---
tags: #DDD 

Exercice de refactoring pour faire émerger progressivement le domaine.
Utilisation de ApprovalTest pour le harnais de tests initiaux

On peut accepter de dégrader / dupliquer le code pendant le refacto pour l'améliorer ensuite.

==> Introduction d'un DSL via des Value Objects pour appliquer des règles de gestion et sécuriser le code

Bouquin : Secure by design

Ajout de tests sur le nouveau code métier :
- Example d'utilisation
- Documentation

Trouver les "quickwins" (commentaires, lignes inutiles, variables inutilisées...) -> "Cleaning the deck"

Rapprocher les déclarations des variables de leur utilisation pour faciliter les refactos.

Pattern sandwich : laisser le code technique autour  du code métier

Regroupement des classes métier en domaines/bounded contexts : 
- Par le son terminal des actions "tion" ou "ing"
- Différents personae

Les 3 complexité du logiciel :
- Essentielle : Intrinsèque au métier (Incompressible)
- Obligatoire : Contraintes d'exploitation, frameworks... (Compressibl)e
- Accidentelle : Erreurs de dev, dette technique (Suppressible)

Specification : Pattern tactique du DDD.
Permet de protéger les invariants du domaine ou de modéliser une règle de gestion.

Ne pas nommer les objets du métier avec le nom du pattern tactique utilisé. Préférer une annotation pour documenter.

Le repository manipule essentiellement des aggregates
Le repository expose essentiellement des aggregate roots
Exemple g'aggregat : Une commande avec ses lignes de commandes. L'aggregate root est l'objet Commande.

Vérifier si on a besoin de services -> si on a trop de services, le modèle devient anémique










