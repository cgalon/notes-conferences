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

# Plugin advanced tables
Pour créer et manipuler des tableaux plus facilement

| Hotkey           | Action                     |
|:---------------- | -------------------------- |
| Tab              | Next Cell                  |
| Shift + Tab      | Previous Cell              |
| Entre            | Next row                   |
| Ctrl + Shift + D | Open table control sidebar |

