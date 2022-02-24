#EventSourcing

Pas besoin de modèles de lecture pour faire de l'Event Sourcing  
Séparer le stream d'évènements en streams spécifiques  
  
On peut remplacer les snapshots par des events d'initialisation d'un nouveau stream.  
  
Pas de modif des events mais des events de correction totale (pas partielle) : 1 event d'annulation + 1 nouvel event corrigé