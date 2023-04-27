---
conference: Devoxx FR
title: Alice au pays d'OpenTelemetry
speaker: Jérome Tama
date: 2023-04-13
video: https://youtu.be/0xSCUgHxZu0
---
tags: #supervision , #openTelemetry , #observabilité , #grafana 

Standard
Convention de désignation des ressources
Instrumentation de plusieurs langages
Collecteur de données

Série de collecteurs composés de receivers, processeurs et exporters

Installation d'un collecteur dans K8S
- Job de collecte de métriques au format Prometheus (toutes les x secondes)
- Processeur
- Exporteur de métriques (au format Prometheus)

Ajout de Prometheus (collecte des métriques)
Ajout d'un Grafana
OpenTelemetry n'est pas un backend de persistance

Besoin de définir les ressources

Définition d'un sidecar pour tous les applications
Les side cars poussent les métriques vers le collecteur maitre

Un pipeline pour les métriques, un pour les traces...

1 daemonset pour collecter les logs et les exporter dans Loki

Pas très rapide à mettre en place




