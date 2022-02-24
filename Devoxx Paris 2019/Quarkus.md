Cloud Native → 12 factors + microservices
#GraalVM  
	Contient plusieurs sous projets  
		Graal Compiler, Substrate VM...  
			Compile plusieurs langages vers du natif  

Quarkus  
	JDK + Graal compiler + Substrate VM  

Substrate VM  
	Elimine tout le code mort  
	Besoin de plein d'options au build  
	Start très rapide  
	Gère la reflexion au coup par coup  

Quarkus  
	Plugin #Maven  
	Hot replace  
	Utilise #CDI  
	Pour les #tests  
		Annotation QuarkusTest  
		RestAssured  
Utilise #Microprofile  
	2 annotations pour faire du streaming avec Kafka (ou RabbitMQ)  
		1 pour le producer  
		1 pour le consumer  
	On peut tester l'application compilée en native  
	Supporte #Prometheus
	