#Docker #Kubernetes #Istio 

## Docker

Mettre à jour la stack #Docker  
Utiliser les multi-stages builds  
Jib ou Kaniko pour réduire les images  
Utiliser une image de base distroless  
gVisor pour la sécurité des images  
  
#Testcontainers pour les tests d'intégration  
  
Paramètres du conteneurs fournis par des variables d'environnement  
Dive pour inspecter les images  
Utiliser des Trusted images  
 
## Kubernetes
  
Utiliser K3S en local  
Sécuriser le dashboard  
Ligne de commandes :  
- Aliases  
- Completion  
- Kubectx  
- Kubens  
- kube-ps1 (ajouter les infos de context k8s dans le prompt  
- kubespy  
- Krew : Package manager pour k8s  
- Stern : mieux que kubectl log  
  
Network policies : pour controler les communications entre les pods  
  
kompose pour traduire des docker-compose  
  
Utiliser kustomize à la place de Helm (kubctl apply -k)  
  
Définir du caping des ressources  
  
Google Cloud Code pour faire plein de manips depuis VSCode et IntelliJ  

## Istio
CLI : istioctl  
  
Outils associés :  
- Jaeger  
- Kiali  
- Grafana  
→ Penser à les configurer et les maintenir