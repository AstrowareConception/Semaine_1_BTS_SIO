# Présentation 7 — Liens, images, chemins et site multi-pages

**Durée cible : environ 55 minutes**  
**Nombre de slides : 22**

---

## Slide 1 — Le Web devient une toile grâce aux liens

Une page isolée peut contenir du texte, des titres et des listes. Mais le Web devient réellement une « toile » lorsque les documents sont reliés entre eux.

Le lien hypertexte permet de passer d'une ressource à une autre. C'est l'une des idées fondatrices du World Wide Web : un document peut pointer vers un autre document, qui peut lui-même pointer vers d'autres ressources.

Cette présentation va nous apprendre à relier des pages, afficher des images et surtout comprendre les **chemins** entre les fichiers.

---

## Slide 2 — La balise `<a>` crée un lien

Un lien HTML utilise l'élément `a`, pour « anchor », ancre.

```html
<a href="https://www.wikipedia.org">Wikipedia</a>
```

Le texte `Wikipedia` est visible et cliquable. L'attribut `href` indique la destination du lien.

On peut lire cette ligne comme une phrase : « crée un lien dont le texte est Wikipedia et dont la destination est cette adresse ».

Comprendre cette lecture est plus utile que recopier la syntaxe mécaniquement.

---

## Slide 3 — `href` contient la destination

Dans :

```html
<a href="https://www.example.com">Visiter le site</a>
```

`href` signifie historiquement « hypertext reference ». Sa valeur indique la ressource vers laquelle le lien pointe.

La destination peut être une URL complète sur Internet, un fichier de votre propre site ou même une partie particulière d'une page.

Cette semaine, nous travaillerons surtout avec deux cas : les liens externes et les liens entre nos propres fichiers HTML.

---

## Slide 4 — Un lien externe utilise généralement une URL complète

Pour pointer vers un autre site, on utilise généralement une adresse complète :

```html
<a href="https://developer.mozilla.org/">MDN Web Docs</a>
```

Le navigateur sait alors qu'il doit demander une ressource située sur un autre service.

**Bonne habitude :** cliquez réellement sur vos liens pendant les tests. Un texte peut sembler correct tout en pointant vers une mauvaise destination.

**Visuel suggéré :** page locale avec une flèche sortant vers un site distant.

---

## Slide 5 — Un lien peut aussi viser un autre fichier local

Si deux fichiers se trouvent dans le même dossier :

```text
mon-site/
├── index.html
└── contact.html
```

alors `index.html` peut contenir :

```html
<a href="contact.html">Contact</a>
```

Aucune URL complète n'est nécessaire. Le navigateur cherche `contact.html` relativement au fichier actuel.

C'est ainsi que nous allons transformer plusieurs pages indépendantes en un petit site cohérent.

---

## Slide 6 — Lire un chemin comme un déplacement

Un chemin relatif peut être lu comme un déplacement dans l'arborescence.

Si nous avons :

```text
mon-site/
├── index.html
└── pages/
    └── formation.html
```

alors depuis `index.html`, le chemin vers `formation.html` est :

```text
pages/formation.html
```

On peut le lire : « entre dans le dossier `pages`, puis ouvre `formation.html` ».

Cette manière de penser évite beaucoup d'erreurs.

---

## Slide 7 — `../` signifie remonter d'un niveau

Imaginons que nous soyons dans `pages/formation.html` et que nous voulions revenir vers `index.html` situé dans le dossier parent.

Le chemin peut s'écrire :

```text
../index.html
```

`..` signifie ici « le dossier parent ».

Nous n'utiliserons pas des arborescences compliquées cette semaine, mais cette notation permet de comprendre pourquoi la position du fichier courant compte dans un chemin relatif.

**Visuel suggéré :** arborescence avec une flèche qui remonte d'un dossier.

---

## Slide 8 — Le même chemin ne fonctionne pas forcément depuis toutes les pages

Considérons :

```text
mon-site/
├── index.html
├── pages/
│   └── formation.html
└── images/
    └── logo.png
```

Depuis `index.html`, l'image se trouve à :

```text
images/logo.png
```

Mais depuis `pages/formation.html`, il faut d'abord remonter :

```text
../images/logo.png
```

Le chemin est donc toujours interprété **depuis l'endroit où se trouve le fichier qui le contient**.

---

## Slide 9 — Erreur classique : copier un chemin sans réfléchir

Un étudiant trouve un lien fonctionnel dans `index.html`, le copie dans une page située dans un sous-dossier, puis constate qu'il ne fonctionne plus.

Le code n'est pas forcément faux en lui-même : le point de départ a changé.

C'est exactement comme une indication routière. « Tournez à droite puis avancez de 100 mètres » n'a de sens que si tout le monde part du même endroit.

**Anecdote pédagogique :** une grande partie des premiers « bugs » Web sont en réalité des problèmes de localisation de fichiers.

---

## Slide 10 — Ajouter une image avec `<img>`

L'élément `img` permet d'intégrer une image dans la page.

```html
<img src="images/photo.jpg" alt="Un ordinateur portable sur un bureau">
```

Contrairement à `p` ou `a`, l'élément `img` n'entoure pas un contenu textuel avec une balise fermante. Il reçoit surtout des informations via ses attributs.

Les deux attributs que nous allons retenir sont `src` et `alt`.

---

## Slide 11 — `src` indique où se trouve l'image

Dans :

```html
<img src="images/photo.jpg" alt="Photo d'un ordinateur">
```

`src` signifie « source ». Sa valeur indique au navigateur où récupérer l'image.

Si le chemin est incorrect, le navigateur ne peut pas afficher le fichier.

La question à se poser est donc toujours : **depuis mon fichier HTML actuel, où se trouve réellement l'image ?**

Cette question résout beaucoup plus de problèmes que de réécrire la balise au hasard.

---

## Slide 12 — `alt` décrit le contenu ou la fonction de l'image

L'attribut `alt` fournit une alternative textuelle à l'image.

```html
<img src="images/logo.png" alt="Logo de l'établissement">
```

Ce texte peut être utile lorsque l'image ne peut pas être vue, notamment pour certaines technologies d'assistance.

Il ne faut pas écrire automatiquement « image de… » si cela n'apporte rien. Le texte doit transmettre l'information importante ou la fonction de l'image dans le contexte.

Nous approfondirons l'accessibilité plus tard, mais prendre cette habitude dès maintenant est utile.

---

## Slide 13 — Une image n'est généralement pas « dans » le HTML

Lorsque votre fichier HTML contient :

```html
<img src="images/chat.jpg" alt="Un chat">
```

le fichier `chat.jpg` n'est pas copié à l'intérieur du HTML. Le document contient une **référence** vers cette ressource.

Le navigateur doit donc réussir à retrouver puis charger l'image séparément.

Cela explique pourquoi envoyer uniquement `index.html` à un camarade ne suffit pas toujours : s'il ne possède pas le dossier `images`, certaines ressources manqueront.

---

## Slide 14 — Organiser les images dans un dossier dédié

Une petite structure propre peut être :

```text
mon-site/
├── index.html
├── formation.html
├── loisirs.html
└── images/
    ├── ordinateur.jpg
    └── sport.jpg
```

Regrouper les images dans un dossier rend le projet plus lisible.

Plus tard, les projets pourront contenir d'autres dossiers : CSS, JavaScript, données ou composants. Pour cette semaine, une structure simple vaut mieux qu'une organisation sophistiquée.

**Règle :** n'ajoutez pas dix dossiers « professionnels » si vous ne comprenez pas encore pourquoi ils existent.

---

## Slide 15 — Noms de fichiers : simples, stables et prévisibles

Pour éviter des problèmes, utilisez des noms simples :

```text
ordinateur.jpg
mon-profil.html
formation.html
```

Évitez pour le moment les espaces, les accents et les noms difficiles à relire comme :

```text
Nouvelle image finale V2 vraiment bonne.JPG
```

Les systèmes peuvent gérer beaucoup de caractères, mais des conventions simples réduisent les erreurs lorsque l'on débute.

**Bonne pratique de classe :** minuscules, mots séparés par des tirets, noms courts mais explicites.

---

## Slide 16 — Attention aux majuscules et minuscules

Sur certains systèmes, `Photo.jpg` et `photo.jpg` peuvent être considérés comme des noms différents.

Un site peut donc sembler fonctionner sur une machine puis échouer après déploiement sur un serveur utilisant une gestion sensible à la casse.

Pour limiter ces surprises, adoptons une convention simple : noms de fichiers en minuscules.

**Exemple :** si le fichier s'appelle `logo.png`, écrivez exactement `logo.png`, pas `Logo.PNG`.

---

## Slide 17 — Créer une navigation commune

Avec trois pages :

```text
index.html
formation.html
loisirs.html
```

on peut ajouter dans chacune :

```html
<nav>
    <a href="index.html">Accueil</a>
    <a href="formation.html">Formation</a>
    <a href="loisirs.html">Loisirs</a>
</nav>
```

L'élément `nav` indique qu'il s'agit d'une zone importante de navigation.

Nous découvrons ici une idée fondamentale : plusieurs pages peuvent partager une structure similaire afin de donner une expérience cohérente à l'utilisateur.

---

## Slide 18 — Un site multi-pages doit permettre de revenir en arrière

Un piège simple consiste à créer un lien depuis l'accueil vers une autre page… mais aucun moyen de revenir.

Techniquement, le bouton « précédent » du navigateur existe. Mais un site doit proposer une navigation compréhensible.

Lors de vos exercices, chaque page devra donc permettre de rejoindre les autres pages principales ou au minimum l'accueil.

**Test simple :** ouvrez directement `loisirs.html`. Pouvez-vous retrouver l'accueil sans modifier l'adresse à la main ?

---

## Slide 19 — Une page peut contenir un lien vers une section interne

Un élément peut recevoir un identifiant :

```html
<h2 id="reseaux">Les réseaux</h2>
```

Puis un lien peut viser ce fragment :

```html
<a href="#reseaux">Aller aux réseaux</a>
```

Cette fonctionnalité n'est pas obligatoire cette semaine. Elle constitue un bon challenge pour les plus rapides et montre qu'un lien peut pointer vers une partie précise d'un document.

---

## Slide 20 — Les liens cassés sont normaux… tant qu'on les teste

Créer plusieurs pages signifie multiplier les chemins possibles. Une faute de frappe ou un fichier déplacé peut casser un lien.

Le professionnel ne suppose donc pas que tout fonctionne : il **teste**.

Cliquez sur chaque lien. Vérifiez chaque image. Essayez d'ouvrir chaque page directement. Revenez vers l'accueil.

Cette démarche de vérification sera réutilisée toute votre carrière, que vous développiez un site, configuriez un réseau ou déployiez un service.

---

## Slide 21 — Exemple d'un petit site complet

```text
mon-premier-site/
├── index.html
├── formation.html
├── loisirs.html
└── images/
    ├── sio.jpg
    └── loisirs.jpg
```

Chaque page contient un titre, quelques paragraphes, éventuellement une liste, puis une navigation permettant de circuler entre les fichiers.

À ce stade, le site peut être visuellement très simple. Ce n'est pas un problème. L'objectif est que sa **structure soit correcte et comprise**.

Le CSS viendra plus tard transformer l'apparence sans remettre en cause cette organisation.

---

## Slide 22 — À retenir : le chemin est une relation entre deux emplacements

Pour réussir les liens et les images, ne mémorisez pas seulement des syntaxes. Posez toujours la même question : **où suis-je et où veux-je aller ?**

`href` indique la destination d'un lien. `src` indique la source d'une ressource comme une image. Les chemins relatifs dépendent de l'emplacement du fichier courant.

À la fin de cette séquence, vous devez pouvoir construire un petit site de plusieurs pages reliées entre elles et contenant des images rangées dans un dossier dédié.

C'est déjà un véritable petit site Web statique.
