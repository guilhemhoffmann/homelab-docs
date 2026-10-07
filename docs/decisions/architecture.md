# Décisions d'architecture

Cette page contient les décisions importantes et surtout **pourquoi** elles ont été prises.

## Format

Pour chaque décision :

### Contexte

Pourquoi le problème existe.

### Options

Les solutions envisagées.

### Décision

Solution retenue.

### Raisons

Pourquoi elle a été retenue.

### Conséquences

Ce que cette décision implique.

---

## Exemple

### Documentation Git + MkDocs

**Contexte :** besoin d'une documentation lisible depuis PC et téléphone.

**Options :**

- Wiki
- Notion
- Git + Markdown
- MkDocs

**Décision :** Git + Markdown + MkDocs.

**Raisons :**

- fichiers versionnés ;
- fonctionnement local ;
- consultation mobile ;
- génération statique ;
- facile à déployer ;
- aucune base de données nécessaire.

**Conséquence :**

La documentation doit rester exploitable sous forme de fichiers Markdown indépendants.
