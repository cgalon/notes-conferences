---
conference: Devoxx FR
title: "L’architecture micro frontend : comment transformer son site web en puzzle géant collaboratif"
speaker: Maxime Ribera et Ludovic Lagatie
date: 2024-04-19
video: https://youtu.be/t4VrZypugA8?si=vpDYeSu83wn60Olv
---
tags: #archi

Ancêtre des microfrontends, les iframes

Mono repo ou multi repo : Les 2 fonctionnent

Rendre les équipes indépendantes et autonomes
Equipes DevOps
Liberté sur les technos
Chaque équipe est responsable de la composition des pages

Choix d'archi : 
- Performance et résilience
- SEO
- Expérience personnalisée
- Migration progressive
- Focus sur la developer XP

Composant principal : Agrégateur

Performance : Récup des MF en asynchrone

Résilience : Certain fragments sont + importants que d'autres
Pareil pour la performance

Mise en place de CSS et JS communs
Lazy load des ressources statiques
On charge d'abord le haut des pages qui est affiché d'abord

Plusieurs solutions ossible : 
Server side rendering
Client side rendering
Hybrid rendering
-> Création d'un arbre de décision pour les équipes

Travail pour que les devs puissent tester en local
Notion "d'expérience" pour surcharger 1 ou x MF sur une infra de recette.
Tous les devs enregistrent leur MF dans une orchestrateur et chaque dev choisi l'expérience qu'il veut utiliser

Pas de MF sans observabilité

Orga des équipes :
- Site owners
- Vertical business owners (fragments principaux de la page)
- Contributeurs
- Micro frontend core team

