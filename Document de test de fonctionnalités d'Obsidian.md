# Plugin Reminder
Pour la gestion de tâches et le rappel associé

- [ ] Tache 1 (@2022-02-22)
- [x] Tache 2 (@2022-02-23)


# Mise en forme de code source

```java

    protected boolean estUnAttributAPrendreEnCompte(UnAttribut attribut) {
        boolean estAPrendreEnCompte = true;
        if (estUnTypeJavaDeBase(attribut)) {
            estAPrendreEnCompte = false;
        }
        else if (estUnTypeExterne(attribut)) {
            estAPrendreEnCompte = false;
        }
        return estAPrendreEnCompte;
    }

```

# Plugin Admonition
Pour l'ajout de notes (à la asciidoctor)
```ad-note
title: Titre de la note
collapse: open
Contenu de la note
Deuxième ligne
```
