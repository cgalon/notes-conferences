* Skaffold
→ ligne de commande  
connait les fichiers importants d'une image (yaml, dockerfile....)  
Encapsule toutes les opérations répétitives  
surveille les modifs du répertoire et les applique automatiquement  
synchronise les pods en local et en distant  

* Distroless  
images plus légères  
plus sécurisées  
flavor :debug pour avoir un shell pour debug à l'intérieur  

* Bazel  
outil de build incémental  
construit des images Docker sans utiliser Docker  
nouveaux fichiers de build et nouvelle syntaxe  

* Jib  
construit des images Docker sans utiliser Docker  
plugin maven ou gradle  
pas besoin de Dockerfile  

* Kaniko  
contruit, dépploi et push une image dans k8s à partir de sources en local  

* kustomize  
customisation de fichiers YAML pour k8s  
pas de templating  
utilise des fichiers de patch  
ne touche pas aux yaml originaux