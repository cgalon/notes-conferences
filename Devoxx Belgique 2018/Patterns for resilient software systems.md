A=1-(1-Ax)² formule pour calculer l'availability d'un composant parallélisé  
  
Stateless services  
Auto-scaling  
CAP theorem (Embrace eventually consistency)  
Decoupling with asynchrone  
Degrade et prioritize traffic with queues (plutôt que de rejeter des requêtes)  
Read/Write sharding (pour les bases distribuées) (permet de mieux gérer les requêtes transactionnelles ou non)  
Database federation  
Database sharding  
Transient state does not belong in databases  
Gérer des timeout sur les transactions  
Augmenter le temps entre chaque retry  
Utiliser jitter (?)  
Idempotent operation (Pasd'effet supplémentaire si on appelle plusieurs fois la même requête avec les même params)  
Circuit breaker  
Creating Resiliency through destruction  
Chaos engineering (simian army Netflix) [http://principlesofchaos.org](http://principlesofchaos.org) [https://chaostoolkit.org](https://chaostoolkit.org)  
Amazon → 100 millisecondes de latence sur la page d'accueil ⇒ Perte de 1% des ventes