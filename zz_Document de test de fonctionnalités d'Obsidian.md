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


# Plugin advanced tables
Pour créer et manipuler des tableaux plus facilement

| Hotkey           | Action                     |
|:---------------- | -------------------------- |
| Tab              | Next Cell                  |
| Shift + Tab      | Previous Cell              |
| Entre            | Next row                   |
| Ctrl + Shift + D | Open table control sidebar |

