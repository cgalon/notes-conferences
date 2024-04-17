---
conference: Devoxx FR
title: SLSA, Sigstore, SBOM and Software Supply Chain Security. Should you care?
speaker: Abdel Sghiouar
date: 2024-04-17
video:
---
tags: #OpenSource , #cicd 

Software supply chain -> chaine de CICD

Attaques sur la supply chain (Log4shell, SolarWinds, Kaseya, Codecov)
81% des bases de codes commerciales ont des failles OSS
Autre exemple : XY Outbreak

Tous les éléments de la chaine de CICD sont des vecteurs d'attaque.

2 bonnes pratiques : Zero Trust et Shift Left

Projet communautaire : Sigstore.dev
-> framework avec plusieurs niveaux de sécurité : Slsa.dev
-> sorte de check-list

SBOM : Software Bill Of Materials
Loi européenne : NIST2
-> Oblige les sociétés à produire les SBOM de leur logiciels
Outil SYFT pour générer des SBOM

SLSA et SBOM sont complémentaires

Outil "cosign" de SIgstore pour signer les images -> standard
Permet d'attacher le SBOM, signer le SBOM...

Possibilité de développer un admition controller sur K8S
Permet de vérifier que les images à déployer sont signées











