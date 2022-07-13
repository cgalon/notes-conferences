---
conference: Devoxx FR
title: Comprendre GraphQL
speaker: Guillaume Scheibel, Geoffroy Couprie
date: 2022-04-20
video: https://www.youtube.com/watch?v=cJzPONmQT3E&list=PLTbQvx84FrARTeUA5pExVR5vjCOqWIplI&index=154
---
tags: #GraphQL , #Kotlin 

#todo Conférence GraphQL à revoir. Arrivé en retard. Raté le début

Le plus important : le schéma

Possibilité de limiter les types utilisés dans le schéma

Le temps de réponse d'une requête dépend de chaque fonction qui y est exécutée
--> Chaque fonction est utilisée en séquentiel

On peut utiliser des directives coté client ou coté serveur

En Kotlin, on peut utiliser des coroutines pour paralléliser les appels et avoir des appels non bloquants.

Les alias permettent de changer le nom en retour des données demandées.
--> Permet au client de définir plsufacilement le format des données en retour

On peut ajouter des directives coté client pour paramétrer, par exemple, les champs à incure ou à exclure. (@include, @skip)

On peut implémeter ses propres directives et définir à quel endroit du schéma elles s'appliquent.

On peut traduire des types complexes "à la volée".
--> Par exemple (et souvent) pour sérialiser le contenu d'un type complexe.

Toutes les reques passent en POST.
Toutes les réponses reviennent en 200 ou 500.

Permet d'avoir des requêtes et des réponses plus complexes.
--> Evite X requêtes équivalentes en REST. 
--> Limite les échanges réseaux

Pas de versionning d'API en GraphQL.

Il existe une notion de "deprecated" sur les données.

On peut composer des graphes issus de plusieurs secteurs/équipes.
--> On a des sous-graphes et un serveur qui agrège tous les résultats.

