---
conference: Devoxx FR
title: Playwright l'outil qui va révolutionner les tests end-to-end
speaker: Jean François Greffier
date: 2023-04-12
video: 
---
tags: #tests 

Soutenu par Microsoft
Automatisation de navigateur
Hérité de Puppeteer

Permet de piloter Safari, Firefox et Chromium depuis leur process de debug
Fonctionne avec Python, Java...

Permet de paralléliser les tests

Axé sur les tests end-to-end
Fournit des assertions utilisables avec PyTest, JUnit, Jest...

Génération de code de test avec Codegen (vers plusieurs langages)
-> Enregistre le parcours utilisateur
-> Reste plus qu'à ajouter des "expect"

Permet d'avoir des locator (sélecteurs) très variés.

Dans une CI, Playwright fournit des traces (sous forme de zip). Contient toutes les commandes exécutées, ce qu'il s'est passé, tout le dom, le source du test utilisé, les messages de la console, vue réseau)
Visualisables avec une app "Trace viewer"
Permet d'analyser et de debugger après coup.

