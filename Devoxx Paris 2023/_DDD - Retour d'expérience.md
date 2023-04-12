---
conference: Devoxx FR
title: DDD - Retour d'expérience
speaker: Thierry Vercruisse
date: 2023-04-11
---
tags: #DDD 

NB : Jounée de la formation Oxiane

# Introduction
 
3 phases dans le DDD : Exploratoire --> Stratégique --> Tactique

DDD EXploratoire :
- Quels besoins?
- Comprendre
- Découvrir
-
DDD stratégique : 
- Décomposer
- Connecter
- Organisation

DDD tactique :
- Définir
- Coder

Expression du problème :
- Qui?
- Quoi?
- Comment?
- Quand?
- Et si?

DDD exploratoire -> Découverte des domaines :
- Modéliser l'état actuel et l'état futur
- Modélisation visuelle

DDD stratégique -> Architecture :
- Def les bounded contexts
- Identifier les Code Domains

DDD Tactique -> Conception technique : 
- Créer des mdèles qui s'alignent

# Le DDD exploratoire

Domin splitting
Comprendre le domaine
Chaque équipe travaile à la définition des domaines
On splitte les bounded context et on les regroupe en identifiant les liens entre eux.	
Deux grandes phases :
- Découverte
- Raffinage du domaine splitting

PLusieurs types d'ateliers :
- Story mapping
- Example mapping
- Capability mapping
L'event storming permet de préciser les 3 ateliers ci-dessus.

Capability mpping (template) : 
- Role/user
	- Client
	- Interne.
	- Partenaire
	- Admin
	- ...
- Description
	- Mon produit est...
	- Mon produit fait
- Capabilities
	- Fonctionnalité
	- Fonctionnalité...
	- --> Regrouper en groupe fonctionnels (bounded contexts)
- Pain points
	- Dette
	- Doc
- Benefits
	- Adoption
	- ...
- Needs
	- Gagner en vélocité
	- ...
- Data consumed
	- Entity IN
- Data produced
	- Entity OUT

D'autres méthodologies : 
- Domain storytelling
- Business Model Canvas
- User journey Mapping
- Pessonae
- ...

Event storming pour raffiner la découverte
- Méthode de brainstorm communicative
- Basé sur les évènement du domaine
- Mais en lumière des process

# DDD stratégique

Identifier des bounded contexts
Donner de l'autonomie en batissant une frontière
1 BC est une frontière autour d'un modèle et de son langage métier conçu dans un but précis

Bounded context canva pour décrire un BC.

Le context mapping permet de définir les intéractions entre 2 BC.
Un ensemble de principes pour maintenir l'intégrité du domaine.
Définit comment les équipes (qui implémentent les BC) vont intéragir entre elles.
Dépendances d'équipes :
- Mutually dependant -> Les merger?
- Free
- Upstream/Downstream -> 1 eq dépend de l'autre 

OHS : Open Host Service -> API
L'équipe qui fournit une API est Upstream

ACL : Anti Corruption Layer
L'équipe qui fournit une ACL est Downstream

CF : Conformist -> Dois suivre les évols des OHS

La context map montre les types d'intéractions entre toutes les équipes 

Classification stratégique
--> Catégorisation en types de domaines : 
- Core (le coeur)
- Support (important)
- Generic (Nécessaire mais pourrait être externalisé)

Source : [ddd-crew]

# DDD tactique

Prendre le temps de concevoir
Choisir le bon blue-print (type d'archi d'iplémentation)
TDD
CI/CD

Utiliser une archi en couches
Isoler le métier

Objectif : cloisement horizontal (couches) + vertical (US)
















