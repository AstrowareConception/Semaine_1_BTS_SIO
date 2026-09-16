# Atelier — Mon premier petit site multi-pages

## Situation

Vous devez créer un petit site présentant un personnage fictif qui vient d'intégrer le BTS SIO.

Le site n'a besoin d'aucun style CSS. Il sera visuellement simple. Nous évaluons aujourd'hui l'organisation du contenu et le fonctionnement des liens.

---

# Étape 1 — Créer exactement l'arborescence demandée

```text
mon_premier_site/
├── index.html
├── formation.html
├── loisirs.html
└── images/
    ├── ordinateur.jpg
    └── loisir.jpg
```

Vous pouvez utiliser deux images libres ou fournies par l'enseignant.

Avant de coder, faites vérifier votre arborescence si vous avez un doute.

---

# Étape 2 — `index.html`

Cette page doit contenir :

- un `title` adapté ;
- un `h1` ;
- deux paragraphes de présentation ;
- une image ;
- une liste de trois objectifs pour l'année ;
- un lien vers `formation.html` ;
- un lien vers `loisirs.html`.

---

# Étape 3 — `formation.html`

Cette page doit contenir :

- un `h1` ;
- un paragraphe expliquant en quelques lignes ce qu'est le BTS SIO ;
- un `h2` « Ce que je souhaite apprendre » ;
- une liste ;
- un lien de retour vers `index.html` ;
- un lien vers `loisirs.html`.

Ne recopiez pas mot pour mot une définition trouvée sur Internet. Reformulez ce que vous avez compris.

---

# Étape 4 — `loisirs.html`

Cette page doit contenir :

- un `h1` ;
- deux `h2` ;
- au moins deux paragraphes ;
- l'image `loisir.jpg` ;
- une liste ordonnée ou non ordonnée ;
- un lien vers `index.html` ;
- un lien vers `formation.html`.

---

# Étape 5 — Ajouter une navigation identique

Lorsque tout fonctionne, essayez d'avoir sur chaque page les trois liens :

```text
Accueil | Formation | Loisirs
```

Exemple :

```html
<nav>
    <a href="index.html">Accueil</a>
    <a href="formation.html">Formation</a>
    <a href="loisirs.html">Loisirs</a>
</nav>
```

Nous utilisons ici `nav` pour représenter une zone de navigation. Vous n'avez pas à apprendre aujourd'hui toutes les balises sémantiques existantes.

---

# Étape 6 — Tester

Vous devez cliquer sur **chaque lien de chaque page**.

Ne considérez pas qu'un lien fonctionne simplement parce que son code « a l'air correct ».

Testez également :

- l'affichage des deux images ;
- la présence des textes `alt` ;
- le titre de l'onglet ;
- l'enregistrement des fichiers.

---

# Étape 7 — Améliorer la lisibilité du code

Ajoutez quelques commentaires utiles :

```html
<!-- Navigation -->
```

```html
<!-- Présentation -->
```

Puis vérifiez l'indentation.

---

# Quand l'atelier est-il terminé ?

Pas lorsque vous avez fini de taper.

Il est terminé lorsque :

- tous les fichiers demandés existent ;
- toutes les pages s'ouvrent ;
- tous les liens ont été testés ;
- toutes les images s'affichent ;
- le contenu respecte l'énoncé ;
- le code est enregistré et lisible.