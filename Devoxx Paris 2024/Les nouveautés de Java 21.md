---
conference: Devoxx FR
title: Les nouveautés de Java 21
speaker: Jean Michel Doudoux
date: 2024-04-18
video: https://youtu.be/3Erjl1862Q4?si=eIDx0G4rsyYUHe8e
---
tags: #Java 

Java 21 en septembre 2023 (LTS)
2 ans entre 2 versions LTS
OpenJDK 21 -> implémentation de référence

# Projet Amber (Evolutions du langage)

Record Patterns
- Permet la déconstruction d'un Record
- On peut imbriquer des Records

Pattern Matching
- Permet de gérer les null dans les switch
- Le compilateur vérifie la dominance des pattern (classes filles avant la classe mère)

String Templates (preview)
- Nouveau type d'expression dans le langage : les templates expressions
- Exemple : String message = STR."Bonjour \{prenom}"
- 3 processeurs de templates par défaut dans le JDK
	- STR
	- FMT
	- RAW
- Possibilité de créer ses propres processeurs de templates

Unamed Classes and Instance Main Methods (preview)
On peut ne plus déclarer une classe qui sert à rien (juste à lancer un traitement)

# Projet Loom

Virtual Threads
- Threads légers gérés par la JVM

Structured Concurrency (preview)

Scoped values

# Ajouts dans le core language

Ajout d'interfaces dans les collections pour uniformiser le comportement


