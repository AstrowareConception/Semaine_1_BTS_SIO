# Mémo HTML — Semaine 1

Ce fichier est un aide-mémoire, pas un texte à apprendre mot pour mot.

# Structure de base

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Titre de la page</title>
</head>
<body>
    <h1>Titre principal</h1>
    <p>Mon contenu.</p>
</body>
</html>
```

# Titres

```html
<h1>Titre principal</h1>
<h2>Partie</h2>
<h3>Sous-partie</h3>
```

# Paragraphe

```html
<p>Mon paragraphe.</p>
```

# Importance et emphase

```html
<strong>Important</strong>
<em>Emphase</em>
```

# Liste non ordonnée

```html
<ul>
    <li>Premier</li>
    <li>Deuxième</li>
</ul>
```

# Liste ordonnée

```html
<ol>
    <li>Étape 1</li>
    <li>Étape 2</li>
</ol>
```

# Lien externe

```html
<a href="https://www.exemple.fr">Visiter le site</a>
```

# Lien vers une page du même dossier

```html
<a href="contact.html">Contact</a>
```

# Image dans un sous-dossier

Arborescence :

```text
site/
├── index.html
└── images/
    └── photo.jpg
```

Code :

```html
<img src="images/photo.jpg" alt="Description de la photo">
```

# Navigation simple

```html
<nav>
    <a href="index.html">Accueil</a>
    <a href="formation.html">Formation</a>
    <a href="loisirs.html">Loisirs</a>
</nav>
```

# Commentaire

```html
<!-- Ceci est un commentaire -->
```

# Cinq vérifications quand quelque chose ne fonctionne pas

1. Le fichier est-il enregistré ?
2. Le nom du fichier est-il exactement correct ?
3. L'extension est-elle correcte ?
4. Le fichier est-il réellement dans le dossier attendu ?
5. Le chemin écrit dans `href` ou `src` correspond-il à l'arborescence ?