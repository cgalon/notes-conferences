---
conference: Devoxx FR
title: Resilience et deisgn patterns pour le cloud
speaker: Sébastien Stormacq
date: 2021-09-29
video: https://www.youtube.com/watch?v=RvxBBQh_uX8&list=PLTbQvx84FrATKYTSVVei8ZouXFGePwSUA&index=12
---
tags: #cloud 

- Répartition géographique des serveurs

- Auto sealing

- Archi asynchrone
	- Découpler le front et le back

- DB
	- Séparation R/W
	- DB séparées par métier
	- Sharding
	- Gérer les timeout de la DB
	- Exponential backoff (pour limiter les retry)

- Idempotence

- Circuit breaker

- Health check

- Load Shedding
	- Rejeter les requêtes client si limite de charge atteinte

- Sharding
	- Sur les serveurs d'app
	- Limiter les impacts de bugs
	- Répartir les clients aléatoirement entre les serveurs

- Chaos engeneering
	- Tester le comportement du système en cas de problème
	- Simian Army

[Doc Amazon](https://aws.amazon.com/fr/architecture/well-architected/)
[Amazon builders library](https://aws.amazon.com/fr/builders-library/?cards-body.sort-by=item.additionalFields.sortDate&cards-body.sort-order=desc&awsf.filter-content-category=*all&awsf.filter-content-type=*all&awsf.filter-content-level=*all)



