# Présentation 6 — Les bases de HTML

**Durée cible : environ 70 minutes**  
**Nombre de slides : 28**

---

## Slide 1 — HTML : structurer le contenu d'une page

HTML signifie **HyperText Markup Language**. Il ne sert pas à « programmer » une page au sens où un langage comme JavaScript ou Python permettrait d'écrire des algorithmes. HTML sert principalement à décrire la structure et le sens du contenu.

Nous allons apprendre à écrire un document minimal, puis à utiliser quelques éléments essentiels : titres, paragraphes, emphase et listes.

Le but n'est pas de mémoriser toutes les balises HTML. Il est de comprendre la logique du langage afin de pouvoir apprendre les autres balises facilement plus tard.

---

## Slide 2 — Une page HTML est d'abord un fichier texte

Un fichier HTML est un fichier texte enregistré avec l'extension `.html`.

Par exemple :

```text
index.html
```

À l'intérieur, nous écrivons du texte ordinaire auquel nous ajoutons des **balises** pour indiquer le rôle des différentes parties.

Le navigateur lit ensuite ce fichier et interprète les balises. Il n'affiche généralement pas les balises elles-mêmes : il utilise leur signification pour construire la page.

**Visuel suggéré :** à gauche du code HTML, à droite le résultat dans un navigateur.

---

## Slide 3 — Une balise ressemble à ceci

Une balise HTML est écrite entre les caractères `<` et `>`.

Par exemple :

```html
<p>
```

La lettre `p` signifie ici « paragraph » : paragraphe.

Beaucoup d'éléments HTML utilisent une balise ouvrante et une balise fermante. La balise fermante contient une barre oblique `/` :

```html
</p>
```

Ces caractères ont un sens précis. Oublier `<`, `>`, `/` ou des guillemets peut modifier la façon dont le navigateur comprend le document.

---

## Slide 4 — Anatomie d'un élément HTML

Prenons :

```html
<p>Bonjour à tous !</p>
```

Nous avons une **balise ouvrante** `<p>`, un **contenu** `Bonjour à tous !`, puis une **balise fermante** `</p>`.

L'ensemble constitue un **élément HTML**.

Cette distinction entre balise et élément est utile. Dans le langage courant, beaucoup de personnes disent « balise » pour parler de l'ensemble, mais techniquement l'élément comprend les balises et son contenu.

**Visuel suggéré :** schéma annoté de l'élément `<p>Bonjour à tous !</p>`.

---

## Slide 5 — Le navigateur cherche une structure

Si nous écrivons simplement :

```text
Bienvenue sur mon site
```

le navigateur peut afficher ce texte, mais nous n'avons pas indiqué sa fonction.

Si nous écrivons :

```html
<h1>Bienvenue sur mon site</h1>
```

nous précisons qu'il s'agit du **titre principal** du document.

HTML ajoute donc du sens au contenu. Le navigateur, les moteurs de recherche et les technologies d'assistance peuvent exploiter cette structure.

---

## Slide 6 — Le squelette minimal d'un document

Nous allons commencer avec cette structure :

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

Elle peut sembler impressionnante pour une première page. Nous allons donc la démonter ligne par ligne. Aucun élément ne doit être recopié comme une formule magique.

---

## Slide 7 — `<!DOCTYPE html>`

La première ligne est :

```html
<!DOCTYPE html>
```

Elle indique au navigateur que le document doit être interprété selon le mode HTML moderne.

Historiquement, les déclarations de type de document étaient plus complexes. Aujourd'hui, cette forme courte suffit pour un document HTML contemporain.

Vous n'avez pas besoin de comprendre l'histoire complète du doctype maintenant. Retenez simplement qu'il doit apparaître au début de vos pages HTML.

**Anecdote :** certaines anciennes pages Web comportaient des doctypes très longs liés à des versions précises de HTML. La syntaxe actuelle est beaucoup plus simple.

---

## Slide 8 — `<html>` : l'élément racine

L'élément `<html>` contient le document HTML.

```html
<html lang="fr">
    ...
</html>
```

L'attribut `lang="fr"` indique ici que la langue principale du document est le français.

Cette information peut être utilisée par des outils d'accessibilité, des navigateurs ou des moteurs de recherche.

Même sur une page très simple, prendre l'habitude d'indiquer correctement la langue fait partie d'une écriture HTML propre.

---

## Slide 9 — Qu'est-ce qu'un attribut ?

Un attribut apporte une information supplémentaire à un élément.

Dans :

```html
<html lang="fr">
```

`lang` est le nom de l'attribut et `fr` sa valeur.

La forme générale que vous rencontrerez souvent ressemble à :

```html
nom="valeur"
```

Les attributs se placent dans la balise ouvrante. Plus tard, `href`, `src` et `alt` deviendront particulièrement importants pour les liens et les images.

---

## Slide 10 — `<head>` : des informations sur la page

L'élément `<head>` contient des informations utiles au document mais qui ne constituent généralement pas le contenu principal affiché dans la page.

On peut notamment y trouver :

```html
<head>
    <meta charset="UTF-8">
    <title>Ma première page</title>
</head>
```

Plus tard, le `head` pourra également contenir des références à des feuilles CSS, des métadonnées ou d'autres ressources.

Pour l'instant, retenons simplement la différence : **head = informations sur le document ; body = contenu visible principal**.

---

## Slide 11 — L'encodage UTF-8

Cette ligne apparaît dans nos pages :

```html
<meta charset="UTF-8">
```

Elle indique l'encodage de caractères utilisé par le document. UTF-8 permet de représenter une immense variété de caractères et de langues.

Sans un encodage correctement interprété, des caractères accentués peuvent apparaître sous une forme étrange.

Vous n'avez pas à apprendre le fonctionnement binaire d'UTF-8 cette semaine. Retenez que cette ligne contribue à afficher correctement le texte de votre page.

---

## Slide 12 — `<title>` n'est pas le titre visible dans la page

L'élément :

```html
<title>Ma première page</title>
```

se trouve dans le `head`. Son contenu est notamment utilisé comme titre de l'onglet du navigateur et lors de l'enregistrement d'un favori.

Il ne remplace pas le titre principal visible dans le contenu de la page.

Pour le titre principal visible, nous utiliserons généralement `<h1>`.

**Piège fréquent :** un étudiant modifie `<title>` puis cherche son nouveau texte dans le corps de la page au lieu de regarder l'onglet du navigateur.

---

## Slide 13 — `<body>` : le contenu affiché

L'élément `<body>` contient le contenu principal présenté à l'utilisateur : textes, titres, images, listes, liens et bien d'autres éléments.

```html
<body>
    <h1>Bonjour le Web !</h1>
    <p>Voici ma première page.</p>
</body>
```

Lorsque vous construisez votre première page, l'essentiel de votre travail se déroule donc dans le `body`.

**Visuel suggéré :** code avec `head` en gris et `body` mis fortement en évidence.

---

## Slide 14 — L'imbrication : des éléments dans des éléments

HTML fonctionne beaucoup par **imbrication**. Un élément peut contenir d'autres éléments.

Le `body` se trouve dans `html`. Un paragraphe peut contenir une emphase. Une liste contient des éléments de liste.

Il faut respecter la logique d'ouverture et de fermeture.

Par exemple :

```html
<p>Bonjour <strong>tout le monde</strong> !</p>
```

L'élément `strong` est entièrement contenu dans le paragraphe.

**Image mentale :** des boîtes placées correctement les unes dans les autres.

---

## Slide 15 — Une mauvaise imbrication crée de la confusion

Regardons :

```html
<p>Bonjour <strong>tout le monde</p></strong>
```

Les éléments se croisent : `strong` est ouvert dans le paragraphe mais fermé après lui. Cette structure est incorrecte.

Une version propre est :

```html
<p>Bonjour <strong>tout le monde</strong></p>
```

Lorsque votre code devient plus long, l'indentation vous aide à repérer ces relations.

---

## Slide 16 — L'indentation rend la structure visible

Comparez :

```html
<body><h1>Titre</h1><p>Texte</p></body>
```

avec :

```html
<body>
    <h1>Titre</h1>
    <p>Texte</p>
</body>
```

Les deux peuvent être compris par le navigateur, mais la seconde forme est beaucoup plus lisible pour un humain.

Le code est lu beaucoup plus souvent qu'il n'est écrit. Une mise en forme claire facilite donc le travail de toute l'équipe, y compris votre futur vous.

---

## Slide 17 — Les titres : `h1` à `h6`

HTML propose six niveaux de titres :

```html
<h1>Titre principal</h1>
<h2>Grande partie</h2>
<h3>Sous-partie</h3>
```

Les nombres représentent des **niveaux hiérarchiques**, pas simplement des tailles de police.

On ne choisit donc pas `h3` parce qu'il paraît visuellement plus petit. On le choisit lorsqu'il représente logiquement un sous-niveau d'un `h2`.

Le CSS permettra plus tard de modifier l'apparence sans détruire la structure logique.

---

## Slide 18 — Un seul plan logique pour le document

Imaginez une dissertation ou un livre : titre, chapitres, sections, sous-sections. HTML suit une logique similaire.

Un document simple peut contenir un `h1`, puis plusieurs `h2`. Chaque `h2` peut éventuellement contenir des sous-parties `h3`.

Cette hiérarchie améliore la compréhension du document, y compris pour certaines technologies d'assistance et pour les moteurs de recherche.

**Exemple :** `h1 = Le BTS SIO`, puis `h2 = Option SLAM`, `h2 = Option SISR`.

---

## Slide 19 — Les paragraphes : `<p>`

Pour un paragraphe, on utilise :

```html
<p>Voici un paragraphe de texte.</p>
```

Chaque idée développée dans un véritable paragraphe peut être placée dans son propre élément `p`.

Évitez de créer artificiellement des paragraphes en ajoutant plusieurs retours à la ligne dans le fichier source. Le navigateur traite les espaces et retours à la ligne HTML différemment d'un traitement de texte.

La structure doit être exprimée par les éléments adaptés.

---

## Slide 20 — Les retours à la ligne du code ne remplacent pas HTML

Si vous écrivez dans votre fichier :

```text
Bonjour
comment
allez-vous ?
```

le navigateur peut regrouper ces espaces et retours à la ligne dans l'affichage.

HTML ne fonctionne pas comme Word. Pour créer des paragraphes, utilisez `<p>`. Pour un véritable retour à la ligne ayant un sens dans le contenu, il existe `<br>`, mais il ne doit pas servir à construire la mise en page générale.

**Règle simple :** ne tapez pas vingt `<br>` pour « pousser » un contenu vers le bas.

---

## Slide 21 — Mettre en évidence une information importante : `<strong>`

L'élément `strong` indique qu'un contenu possède une forte importance.

```html
<p>N'oubliez pas de <strong>sauvegarder votre fichier</strong>.</p>
```

Les navigateurs affichent généralement ce contenu en gras, mais le sens est plus important que l'apparence.

Si votre seul objectif est « je veux du gras parce que c'est joli », cette question relèvera plutôt de la présentation CSS.

HTML cherche d'abord à décrire la signification du contenu.

---

## Slide 22 — Mettre une emphase : `<em>`

L'élément `em` sert à marquer une emphase dans une phrase.

```html
<p>Je veux <em>vraiment</em> comprendre ce code.</p>
```

Il est généralement affiché en italique, mais là encore, l'apparence n'est pas l'idée principale.

Lire la phrase à voix haute permet de sentir le rôle de l'emphase : on insiste sur le mot concerné.

**Exemple oral :** « Je n'ai pas dit qu'il avait volé le fichier » peut changer de sens selon le mot sur lequel on insiste.

---

## Slide 23 — Les listes non ordonnées : `<ul>`

Une liste non ordonnée est adaptée lorsque l'ordre des éléments n'est pas essentiel.

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

`ul` signifie « unordered list ». Chaque élément de la liste est placé dans un `li`, « list item ».

Un navigateur représente généralement cette liste avec des puces.

**Exemple :** une liste de technologies connues ou une liste de centres d'intérêt.

---

## Slide 24 — Les listes ordonnées : `<ol>`

Une liste ordonnée est pertinente lorsque l'ordre possède un sens.

```html
<ol>
    <li>Créer le fichier</li>
    <li>Écrire le HTML</li>
    <li>Enregistrer</li>
    <li>Actualiser le navigateur</li>
</ol>
```

`ol` signifie « ordered list ».

Le choix entre `ul` et `ol` ne dépend donc pas seulement de l'apparence souhaitée. Posez-vous la question : **si je mélange les éléments, est-ce que le sens change ?** Si oui, une liste ordonnée peut être appropriée.

---

## Slide 25 — Une liste contient des `li`

Une erreur fréquente consiste à écrire directement du texte dans une liste sans créer correctement les éléments de liste.

Structure attendue :

```html
<ul>
    <li>Réseau</li>
    <li>Développement</li>
</ul>
```

Le `ul` ou le `ol` joue le rôle de conteneur. Les `li` représentent les éléments.

Cette structure illustre à nouveau le principe d'imbrication : un élément en contient d'autres selon des règles précises.

---

## Slide 26 — Une première page complète

Nous pouvons déjà produire une page structurée :

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Découverte du BTS SIO</title>
</head>
<body>
    <h1>Le BTS SIO</h1>
    <p>Je découvre ma première page HTML.</p>

    <h2>Ce que je vais apprendre</h2>
    <ul>
        <li>Le développement</li>
        <li>Les réseaux</li>
        <li>La cybersécurité</li>
    </ul>
</body>
</html>
```

Chaque ligne doit maintenant avoir un sens pour vous.

---

## Slide 27 — Le navigateur est tolérant, mais nous devons rester rigoureux

Les navigateurs essaient souvent de réparer ou d'interpréter du HTML imparfait. Une page peut donc « avoir l'air de marcher » malgré certaines erreurs.

Cela ne signifie pas que le code est correct.

Prendre de bonnes habitudes dès le début permet d'éviter des problèmes plus difficiles lorsque les documents deviennent complexes : fermer les éléments correctement, respecter l'imbrication, indenter et utiliser les éléments pour leur sens.

**Anecdote de terrain :** « Ça s'affiche » et « c'est correctement écrit » sont deux affirmations différentes.

---

## Slide 28 — Le socle HTML à retenir aujourd'hui

Vous n'avez pas besoin de mémoriser cinquante balises. Pour l'instant, le socle est très petit :

`<!DOCTYPE html>`, `html`, `head`, `meta`, `title`, `body`, `h1`, `h2`, `h3`, `p`, `strong`, `em`, `ul`, `ol` et `li`.

Surtout, vous devez comprendre les concepts derrière ces éléments : **document, structure, élément, balise ouvrante, balise fermante, attribut, imbrication et hiérarchie**.

À partir de cette logique, nous pouvons maintenant rendre nos pages réellement reliées entre elles grâce aux liens et y intégrer des images.
