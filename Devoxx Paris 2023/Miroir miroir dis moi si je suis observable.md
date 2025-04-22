---
conference: Devoxx FR
title: Miroir, miroir dis moi si je suis observable
speaker: Virginie Hang et Robin Sooprayen
date: 2023-04-14
video: https://youtu.be/PEDHMxNc-NA
---
tags: #observabilité , #supervision , #Monitoring , #openTelemetry , #métriques 

Premier dashboard "au doigt mouillé"
Alerting automatique 
=> toujours autant d'incidents

Manque d'observabilité (logs...)

Appliquer la méthode FMEA (Failure mode and effects analysis)
=> Amélioration du MTTR

SRE : Service Reliability Engineering
SLI (service level indicator) et SLO (service level objectif)
Mettre de l'alerting si les SLO sont dépassés

Développement de l'application
-> Plus complexe, plus dure à troubleshooter

Ajout d'openTelemerty pour traiter les traces
Pas d'auto instrumentation du code -> custom -> pour avoir des traces plus utiles
Collecte avec OpenTelemerty
Exploitation avec Jaeger (corrèle les traces et les logs)
Grafana permet aussi de visualiser les traces












