# Premiers pas en HTML

## 1. À quoi sert HTML ?

HTML signifie **HyperText Markup Language**.

HTML sert à décrire la structure et le sens du contenu d'un document Web.

Pour cette première approche :

- **HTML** : structure et contenu ;
- **CSS** : présentation ;
- **JavaScript** : comportements et programmation côté navigateur.

Cette semaine, nous nous concentrons sur HTML.

---

## 2. Une première page

Écrivez progressivement :

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Ma première page</title>
</head>
<body>
    <h1>Bonjour le Web !</h1>
    <p>Ma première page HTML.</p>
</body>
</html>
```

Ne vous contentez pas de copier. Nous allons expliquer chaque partie.

### `<!DOCTYPE html>`

Indique que le document utilise HTML moderne.

### `<html lang="fr">`

Élément principal de la page. L'attribut `lang="fr"` indique que le contenu principal est en français.

### `<head>`

Contient des informations concernant le document qui ne constituent pas directement le contenu principal affiché dans la page.

### `<meta charset="UTF-8">`

Indique l'encodage utilisé. UTF-8 permet notamment de gérer correctement de très nombreux caractères.

### `<title>`

Définit notamment le titre visible dans l'onglet du navigateur.

### `<body>`

Contient le contenu affiché de la page.

---

# 3. Balises ouvrantes et fermantes

Exemple :

```html
<p>Bonjour</p>
```

- `<p>` ouvre le paragraphe ;
- `Bonjour` est son contenu ;
- `</p>` ferme le paragraphe.

Certaines constructions, comme `img`, fonctionnent différemment et ne possèdent pas cette paire ouvrante/fermante.

---

# 4. Titres

HTML dispose de niveaux de titres :

```html
<h1>Titre principal</h1>
<h2>Une grande partie</h2>
<h3>Une sous-partie</h3>
```

On choisit un niveau pour représenter la **structure du document**, pas simplement parce qu'un texte paraît plus gros ou plus petit.

---

# 5. Paragraphes

```html
<p>Voici un paragraphe.</p>
<p>Voici un deuxième paragraphe.</p>
```

---

# 6. Mettre en évidence du contenu

```html
<p>Ce point est <strong>important</strong>.</p>
<p>Ce terme peut recevoir une <em>emphase</em>.</p>
```

---

# 7. Listes non ordonnées

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

Utilisez une liste non ordonnée lorsque l'ordre des éléments n'est pas essentiel.

---

# 8. Listes ordonnées

```html
<ol>
    <li>Créer le dossier</li>
    <li>Créer index.html</li>
    <li>Écrire le contenu</li>
</ol>
```

Ici, l'ordre a un sens.

---

# 9. Liens

```html
<a href="https://www.wikipedia.org">Visiter Wikipédia</a>
```

- `a` crée le lien ;
- `href` indique la destination ;
- le texte entre les balises est le texte cliquable.

Vers une autre page située dans le même dossier :

```html
<a href="contact.html">Contact</a>
```

---

# 10. Images

Si votre arborescence est :

```text
mon-site/
├── index.html
└── images/
    └── ordinateur.jpg
```

vous pouvez écrire :

```html
<img src="images/ordinateur.jpg" alt="Un ordinateur portable">
```

`src` indique où trouver l'image.

`alt` fournit une alternative textuelle. Ne le considérez pas comme un détail facultatif.

---

# 11. Comprendre un chemin relatif

Depuis `index.html`, le chemin :

```text
images/ordinateur.jpg
```

signifie en substance :

> pars du dossier actuel, entre dans `images`, puis trouve `ordinateur.jpg`.

Si vous déplacez le fichier, le chemin peut devenir faux.

---

# 12. Indentation

Préférez :

```html
<ul>
    <li>Premier élément</li>
    <li>Deuxième élément</li>
</ul>
```

à :

```html
<ul><li>Premier élément</li><li>Deuxième élément</li></ul>
```

Le navigateur peut parfois comprendre les deux, mais les humains doivent pouvoir relire facilement votre code.