---
conference: Devoxx FR
title: Creating a documentation site for users with AsciiDoc and Antora
speaker: Alexander Schwartz
date: 2024-04-17
video:
---
tags: #livingdoc , #antora

Une site de doc utile :
- Du contenu simple à "scanner"
- Bonne navigation
- Recurring structure
- Recherche intégrée au site

Construire une page comme si c'était la première page que l'on voit : 
- Contexte sur chaque page
- ...
- #TODO A compléter avec la vidéo du site

Antora fournit des outils de publication et une structure de doc
Peut collecter des docs depuis plusieurs repos
Utilise Asciidoc
Créer un site statique

Modulaire et extensible

Le plugin IntelliJ pour Asciidoc supporte Antora

Antora structure la doc en composants qui contiennent des modules qui contiennent les items (pages, images...)

Antora utilise un playbook qui contient la liste des repos à prendre en compte.
Pendant le run :
- Clone les repos
- Crée les HTML
- Merge les docs générés avec le theme choisi
- Crée un index pour la recherche
- Crée le site en sortie


