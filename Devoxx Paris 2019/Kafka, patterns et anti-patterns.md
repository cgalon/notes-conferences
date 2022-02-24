#Kafka 

Penser à la durabilité  
→ Réplication entre multiples clusters  
→ acks=all  
→ min.insync.replicas = 2  
  
Mécanisme de retry built-in dans l'API producer