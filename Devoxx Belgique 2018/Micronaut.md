Supporte #Java, #Groovy et #Kotlin  
Dependency injection  
Pas de reflection ou de runtime proxies  
Basé sur Netty  
  
CLI téléchargeable via sdkman  
  
Création d'un controleur comme dans #SpringBoot  
  
Propose un server “embedded” pour faire des TIC rapidement  
@MicronautTest pemet d'encapsuler la création du serveur de test  
  
Utilise Consul de manière transparente  
Possibilité de variabiliser le path des ressources REST (et d'avoir une valeur par défaut)  
  
@Fallback permet d'implémenter une stratégie de fallback sur une ressource en utilisant une classe avec la même interface  
@CircuitBreaker permet de définir un circuit breaker sur une ressource  
  
Supporte GraalVM et les native-image de #GraalVM  
Permet de créer une application native qui démarre super vite (pour un service simple 19ms au lieu de 1500ms avec la JVM)