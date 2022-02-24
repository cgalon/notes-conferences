#Java #Docker 

Frameworks : #Quarkus, Helidon (?)  
  
But : Avoir des images légères et donc des layers légers  
  
Mettre les dépendances dans un layer spécifique  
Layers spécifiques pour tout ce qui est statique  
  
Regarder fn (fnproject sur GitHub)  
  
dive pour regarder les layers des images  
  
CDS : Outil du JDK pour compiler et créer des exécutable plus rapides  
  
Evolutions en cours pour que la JVM sache qu'elle tourne dans des conteneurs et soit plus performante  
  
Résumé des outils :  
• jlink  
• jlink compression  
• Graal native-image  
• CDS  
• Portola  
• Distroless images  
• Ergonomic  
  
Pour la securité :  
• Docker-bench-security  
• Snyk  
• #Clair  
• Anchroe
