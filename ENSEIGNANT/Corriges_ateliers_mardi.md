# Corrigés et conseils d'animation — Mardi

Ce fichier accompagne les ateliers manipulables placés dans `JOUR_2_MARDI/ATELIERS`.

# Mission 1 — Le code en désordre

Ordre attendu :

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Ma première page</title>
</head>
<body>
    <h1>Bonjour le Web !</h1>
</body>
</html>
```

Faire verbaliser la séparation entre les informations placées dans `head` et le contenu principal placé dans `body`.

# Mission 2 — La page cassée

Erreurs principales :

1. `h1` se ferme avec `h2` au lieu de `h1` ;
2. le premier paragraphe utilise une seconde balise ouvrante au lieu de `</p>` ;
3. `strong` et `p` sont mal imbriqués ;
4. les éléments `li` ne sont pas fermés ;
5. la liste commence avec `ul` mais se termine avec `ol` ;
6. le lien `a` n'est pas fermé.

Le navigateur peut afficher une page malgré certaines erreurs. Ne pas confondre « quelque chose apparaît » et « la structure est correctement écrite ».

# Mission 3 — Le mystère des chemins

Dans `index.html` :

```html
<a href="pages/profil.html">Découvrir le profil du robot</a>
<img src="images/robot.svg" alt="Petit robot pédagogique tenant une loupe">
```

Dans `pages/profil.html` :

```html
<img src="../images/robot.svg" alt="Petit robot pédagogique tenant une loupe">
<a href="../index.html">Revenir à l'accueil</a>
```

Le point de départ du chemin change selon l'emplacement du fichier HTML qui contient le chemin.

# Mission finale

Il n'existe pas de correction unique. Valider les éléments suivants :

- la structure minimale est complète ;
- le contenu respecte la hiérarchie des titres ;
- la liste choisie correspond au sens ;
- le lien fonctionne ;
- l'image locale s'affiche ;
- `alt` transmet une information utile ;
- les balises sont fermées et correctement imbriquées ;
- l'étudiant sait expliquer plusieurs lignes de son code.

Pendant la relecture croisée, l'observateur ne prend pas le clavier du pilote.
