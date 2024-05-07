---
conference: Devoxx FR
title: Panorama des risques, vulnérabilités et pistes pour une utilisation plus sûre de l'IA générative
speaker: Willy Malvault, Aurélien Fournet
date: 2024-04-18
video: https://youtu.be/eD6Tuh0irPc?si=mmCEeZ1j_m7lSShs
---
tags: #ia 

Techno en cours de maturation

Cadre réglementaire + Analyse de risques = Mesures de protection
Cf. IA Act

![[20240418_114540.jpg]]
# Risque comportemental et social

Risque accru sur la désinformation (hallucinations)
Deepfake et phishing
Risque de comportement inadapté
Impact environnemental et techno lucidité

# Risques liés au contrôle et à la validation des LLM

![[20240418_115349.jpg]]

Le but est de coder mieux, pas plus vite
Une IA est pas programmée pour "désapprendre"
Vulnérabilité des LLMs à l'injection de prompt
Chercher "jailbreak prompt" sur Google
Sur Hugging fac plus de 100 modèles malveillants (Exemple Backdoor Wiz)
Le retour des Worms (vers) propagés par les LLM

Exemple de résultat d'analyse de risque :
![[20240418_120438.jpg]]
# Mesure de protection

Il faut commencer par la gouvernance
- Sélectionner et prioriser les cas d'usage
- Mise en conformité avec les politiques de sécurité

Protection par contrôle périphérique
- Utilisation d'un proxy LLM
- Par exemple LLM Guard
- Utilisation d'un LLM pour analyser les injections de prompt

Les promesses de tenant et d'isolation
- Isolation complète ?
- Confiance au provider ?
- Chez BPI quelques requêtes suspectes venant des grands fournisseurs d'IA Gen

Données partagées + RAG = Problème relou

Lutter contre le shadow IA Gen
-> Solution collaborative (sensibilisation + blocage occasionnel)

Article LinkedIn : 
![[20240418_121724.jpg]]










