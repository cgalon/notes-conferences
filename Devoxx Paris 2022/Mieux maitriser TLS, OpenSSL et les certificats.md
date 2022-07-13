---
conference: Devoxx FR
title: Mieux maitriser TLS, OpenSSL et les certificats
speaker: Mathieu Humbert
date: 2022-04-22
video: https://www.youtube.com/watch?v=P6brMpIZaOo&list=PLTbQvx84FrARTeUA5pExVR5vjCOqWIplI&index=144
---
tags: #TLS

TLS successeur de SSL

3 piliers :
- Confidentialité
- Authentification
- Intégrité

TLS utilise un protocole asym pour init puis symétrique

Phase de Handshake (init) 
- Accord sur la Cipher suite à utiliser
- Echange de clé

TLS 1.2 : 2 A/R
TLS 1.3 : 1 A/R

Cipher Suite : Suite de caractères contenant
- Key exchange
- Authentication
- Cipher
- MAC


