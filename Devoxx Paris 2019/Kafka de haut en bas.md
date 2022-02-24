Bus de messages  
ETL (Kafka connect)  
Créé par LinkedIn  
Persistance, durabilité des messages  
Scalable  
#Kafka streams  
KSQL pour processer la données  
  
On peut utiliser Kafka connect pour récupérer des données de prod et les anonymiser  
  
Définir la durée de rétention des messages (TTL)  
  
Sécurité des accès aux données  
  
Message = Header + Key + Value  
  
1 topic regroupe plusieurs partitions. 1 partition regroupe plusieurs segments  
  
Utilise #ZooKeeper en interne pour faire fonctionner le controler  
  
Plusieurs niveaux d'acquittement pour l'insertion des données. (toujours utiliser ack=all → Veut dire que le leader et les brokers ont stocké la donnée) (et utiliser la propriété min.insyc.replica)  
  
On peut regrouper les consumers par groupe  
  
Apache Kafka → Brique de base  
Plateforme Confluent amène d'autres briques :  
→ Connectivité  
→ KSQL, ...  
  
Bonne pratique : Mettre Kafka en front d'Elastic Search et Log Stash  
Logstash pour vider une table de DB vers Kafka → Pas très scalable, pas de faul tolerance  
  
Kafka Connect permet l'import/export de données de/vers des bases de données  
DBezium utilise les journaux des bases pour récupérer des infos plutôt que faire des select * from ...  
  
Kafka Streams offre une API de streaming de données au dessus de l'API de base de Kafka  
  
Interactive queries  
  
Utilisation Kafka SQL  
→ Plus simple que Kafka Stream  
→ Les requêtes rendent un stream de valeurss. Ne s'arrêtent pas comme du SQL classique.  
→ On peut aussi avoir un seul résultat au lieu d'un stream → Notion de TABLE  
→ Transpiler entre du SQL et Kafka Stream  
[www.conlfluent.io/stream-processing-cookbok](http://www.conlfluent.io/stream-processing-cookbok)  
  
Il existe une distribution de Confluent pour tout avoir et tout lancer en même temps  
Image #Docker  
Confluent Operator ( #Kubernetes ) 
  
Schema registry : Gouverance de la data  
  
#Monitoring : Confluent Control Center  
  
Ressources : Blog de Confluent, WhitePaper  
  
[https://github.com/confluentinc/cp-demo](https://github.com/confluentinc/cp-demo) : Démo à télécharger pour tout démarrer d'un coup