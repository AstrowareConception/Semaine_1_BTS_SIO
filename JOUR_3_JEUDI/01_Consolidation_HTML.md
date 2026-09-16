# Consolidation HTML

# 1. Refaire avant d'ajouter

Créez un nouveau dossier :

```text
jeudi_revisions
```

Puis un fichier `index.html`.

Sans recopier immédiatement le cours, essayez de reconstruire :

- le doctype ;
- `html` ;
- `head` ;
- l'encodage UTF-8 ;
- `title` ;
- `body` ;
- un `h1` ;
- un paragraphe.

Après quelques minutes, comparez avec le [mémo HTML](../RESSOURCES/Memo_HTML.md).

Corrigez votre travail au lieu de supprimer le fichier.

---

# 2. Ajouter une structure de contenu

Votre page doit maintenant comporter :

```text
Titre principal
Présentation
Ce que j'ai appris lundi
Ce que j'ai appris mardi
Trois notions à retravailler
```

Choisissez les balises adaptées parmi celles vues mardi.

---

# 3. Créer une seconde page

Dans le même dossier, créez :

```text
formation.html
```

Vous avez maintenant :

```text
jeudi_revisions/
├── index.html
└── formation.html
```

Dans `index.html` :

```html
<a href="formation.html">Découvrir la formation</a>
```

Dans `formation.html` :

```html
<a href="index.html">Retour à l'accueil</a>
```

Testez les **deux directions**.

---

# 4. Ajouter une troisième page

Créez :

```text
loisirs.html
```

Ajoutez des liens entre les trois pages.

Vous découvrez ici une première forme très simple de navigation.

---

# 5. Ajouter un dossier d'images

Votre projet doit devenir :

```text
jeudi_revisions/
├── index.html
├── formation.html
├── loisirs.html
└── images/
    └── illustration.jpg
```

Affichez `illustration.jpg` depuis `index.html`.

Puis essayez de l'afficher aussi depuis `formation.html`.

Observez : puisque les deux fichiers HTML sont dans le même dossier, le chemin vers `images/illustration.jpg` est identique.

---

# 6. Commentaires HTML

Nouvelle notion du jour :

```html
<!-- Ceci est un commentaire HTML -->
```

Un commentaire permet d'écrire une information dans le fichier source sans qu'elle apparaisse comme contenu normal dans la page.

Vous pouvez organiser votre fichier :

```html
<!-- Navigation -->

<!-- Présentation -->

<!-- Liste des apprentissages -->
```

N'abusez pas des commentaires. Ils doivent aider à comprendre, pas répéter l'évidence.

---

# 7. Petits incidents à résoudre

Pour chacun, essayez d'expliquer le problème avant de modifier quoi que ce soit.

## Cas A

Le fichier réel s'appelle :

```text
formation.html
```

Le lien contient :

```html
<a href="formations.html">Formation</a>
```

Que remarquez-vous ?

## Cas B

L'image est ici :

```text
images/ordinateur.jpg
```

Le code contient :

```html
<img src="ordinateur.jpg" alt="Ordinateur">
```

Que manque-t-il ?

## Cas C

Vous venez de modifier un texte dans VS Code, mais le navigateur affiche encore l'ancien texte.

Avant de chercher une erreur compliquée, quelle vérification très simple devez-vous effectuer ?

## Cas D

Vous avez créé `contact.html`, mais vous êtes en train de modifier une ancienne copie du projet située sur le Bureau.

Pourquoi est-il important de toujours savoir **quel dossier de projet** est ouvert dans VS Code ?