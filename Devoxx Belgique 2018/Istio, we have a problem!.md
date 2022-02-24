Visibilité sur les traces distribuées, les endpoints, ce qui est déployé sur K8S  
  
#Istio injecte un http proxy dans chaque pod  
  
→ Pemet de savoir ce qui est installé, ce qui transite → qui fait quoi  
→ Fournit des dashboards Grafana (niveau applicatif, codes retour http, tps d'exec...)  
→ Permet de voir les traces applicatives (entrées / sorties http)  
→ Permet de déployer en Canary release  
→ Envoyer une copie du traficà une autre version (après une canary release, le temps de tester en plus grand)  
→ Blue/Green deploiement  
→ SSL transparent entre les services (Les Envoy communiquent en TLS)