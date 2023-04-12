---
conference: Devoxx FR
title: Grafana Loki comme Prometheus mais pour les logs
speaker: Cyril Tovena
date: 2023-04-12
video: 
---
tags: #log , #loki , #grafana

Solution intégrée aux outils cloud (grafana, k8s, prometheus)
Outil dédié aux logs

Corréler les métriques et les logs

Les agents installés sur les nodes (Fluentbit...) envoient les logs à Loki
Loki gère plusieurs clusters
Plusieurs clients possibles : Grafana, AlertManager, API...

Loki n'indexe pas le contenu des logs. Seules les entrées sont indexées.
Loki indexe les timestamps et les labels
-> Supporte bien la charge

Dans Loki, on commence déjà par restreindre la recherche (intervalle de temps, cluster, namespace...)
Langage : LogQL inspiré par PromQL

Intégré à Grafana. Garde les même critères de recherche quand on passe de Grafana à Loki

Passage transparent etre métriques et logs.
On peut intégrer des logs dans les dashboards Grafana.

NB : Plus convivial que Kibana

