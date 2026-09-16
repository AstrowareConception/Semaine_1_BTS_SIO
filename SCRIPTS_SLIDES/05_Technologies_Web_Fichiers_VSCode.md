# Présentation 5 — De quoi est faite une page Web ? Fichiers, dossiers et VS Code

**Durée cible : environ 50 minutes**  
**Nombre de slides : 20**

---

## Slide 1 — Passer de l'utilisateur au créateur

Jusqu'ici, nous avons surtout observé le Web du point de vue de l'utilisateur : un navigateur demande des ressources et un serveur lui répond.

Nous allons maintenant changer de côté. Pour créer une page Web, il faut comprendre de quoi elle est faite, où se trouvent ses fichiers et comment les modifier proprement.

Cette transition est importante : un site n'est pas une image magique stockée quelque part sur Internet. C'est un ensemble organisé de ressources que le navigateur reçoit puis interprète.

**Visuel suggéré :** écran partagé « utilisateur » à gauche, « créateur » à droite.

---

## Slide 2 — Trois technologies que vous rencontrerez partout

Le Web moderne repose notamment sur trois technologies fondamentales côté navigateur : **HTML, CSS et JavaScript**.

HTML décrit la structure et le sens du contenu. CSS gère principalement la présentation visuelle. JavaScript permet d'ajouter des comportements et de la logique exécutée dans le navigateur.

On les apprend souvent ensemble, mais il est préférable de les distinguer clairement dès le départ. Cette semaine, nous allons surtout travailler HTML afin de comprendre la structure avant de nous préoccuper de l'apparence ou de l'interactivité.

---

## Slide 3 — HTML : la structure du document

HTML signifie **HyperText Markup Language**. C'est un langage de balisage utilisé pour structurer le contenu d'une page Web.

Avec HTML, on indique par exemple : « ceci est le titre principal », « ceci est un paragraphe », « ceci est une liste », « ceci est un lien » ou « cette ressource est une image ».

HTML ne sert donc pas principalement à dire qu'un texte doit être bleu ou qu'un bouton doit être arrondi. Il sert d'abord à décrire **ce qu'est le contenu**.

**Visuel suggéré :** article de journal avec titre, paragraphes, image et liste reliés à leurs balises HTML.

---

## Slide 4 — CSS : la présentation

CSS signifie **Cascading Style Sheets**. Il permet de contrôler l'apparence : couleurs, tailles, espacements, alignements, mise en page ou adaptation aux différentes tailles d'écran.

Un même document HTML peut être présenté de manières très différentes grâce au CSS.

Cette séparation est importante : la structure du contenu ne devrait pas dépendre entièrement de son apparence.

**Anecdote historique :** le besoin d'un langage de feuilles de style pour le Web apparaît très tôt. Håkon Wium Lie propose les Cascading Style Sheets en 1994 alors qu'il travaille au CERN.

---

## Slide 5 — JavaScript : le comportement

JavaScript permet d'ajouter des comportements programmés dans une page : réagir à un clic, modifier du contenu, vérifier un formulaire, récupérer des données depuis un serveur ou construire une application interactive.

Le JavaScript moderne permet de réaliser des applications très complexes directement dans le navigateur.

Mais apprendre les trois technologies en même temps serait inutilement difficile pour une première semaine. Nous allons donc poser une fondation solide en HTML avant d'ajouter plus tard la présentation et la programmation.

---

## Slide 6 — Une analogie utile… à ne pas prendre au pied de la lettre

On compare souvent une page Web à une maison.

HTML serait la structure : pièces, murs, portes. CSS serait la décoration et l'aménagement. JavaScript serait ce qui permet aux équipements d'agir : interrupteurs, portes automatiques ou thermostat.

Cette analogie aide à distinguer les rôles, même si elle reste simplifiée.

L'idée principale est que ces technologies coopèrent sans être interchangeables. Utiliser HTML uniquement pour obtenir un effet visuel peut produire une structure incorrecte, tout comme décorer une maison ne remplace pas ses murs porteurs.

---

## Slide 7 — Voir le code source change le regard

Dans un navigateur, l'utilisateur voit le résultat final. Pourtant, il est possible d'afficher le code source HTML reçu pour une page.

Ce code paraît parfois impressionnant sur un grand site moderne, mais vous y retrouverez progressivement des structures familières : titres, paragraphes, liens, images et références à d'autres ressources.

Le premier objectif n'est pas de comprendre tout le code d'un grand site. Il est de réaliser que le navigateur travaille à partir de textes structurés et de ressources, pas d'une capture d'écran envoyée par le serveur.

---

## Slide 8 — Avant de coder : comprendre fichiers et dossiers

Un grand nombre de difficultés de débutants en développement Web ne viennent pas réellement de HTML. Elles viennent d'une mauvaise compréhension des fichiers, dossiers et chemins.

Si votre code demande une image qui n'est pas dans le dossier prévu, le navigateur ne peut pas l'inventer. Si vous modifiez un autre fichier que celui que vous ouvrez, vos changements semblent ne jamais apparaître.

Maîtriser le système de fichiers est donc une compétence technique fondamentale, pas un détail administratif.

---

## Slide 9 — Qu'est-ce qu'un fichier ?

Un fichier est un ensemble de données enregistré sous un nom. Il peut contenir du texte, une image, du son, une vidéo ou un programme.

Un fichier HTML est principalement un fichier texte contenant du balisage HTML.

Par exemple : `index.html`.

Le nom comporte ici deux parties visibles : `index`, choisi pour identifier le fichier, et `.html`, l'extension indiquant son type.

**Visuel suggéré :** plusieurs fichiers avec extensions `.html`, `.jpg`, `.png`, `.txt`, `.pdf`.

---

## Slide 10 — Les extensions sont importantes

Sous Windows, les extensions des fichiers connus peuvent parfois être masquées. Cela conduit à un piège classique : penser avoir créé `index.html` alors que le fichier s'appelle réellement `index.html.txt`.

Pour un navigateur, ces deux noms sont différents. Le second reste un fichier texte portant une extension supplémentaire.

Pendant les travaux pratiques, il faudra donc être attentif aux noms exacts des fichiers et à leurs extensions.

**Anecdote de terrain :** une quantité surprenante de « bugs HTML » disparaissent simplement en affichant les extensions de fichiers.

---

## Slide 11 — Les dossiers organisent les fichiers

Un dossier permet de regrouper des fichiers et d'autres dossiers. Un petit site peut être organisé ainsi :

```text
mon-site/
├── index.html
├── contact.html
└── images/
    └── logo.png
```

Cette arborescence indique que `index.html` et `contact.html` sont au même niveau, tandis que `logo.png` est contenu dans le sous-dossier `images`.

Lire une arborescence deviendra aussi naturel que lire une table des matières.

---

## Slide 12 — Le dossier du projet est votre point de repère

Lorsque vous commencez un exercice, créez un dossier clairement nommé et conservez toutes les ressources du projet à l'intérieur.

Évitez de disperser `index.html` sur le Bureau, une image dans Téléchargements et une seconde page dans Documents. Une telle organisation rend les chemins difficiles à comprendre et complique les échanges avec un camarade.

Un projet bien rangé facilite déjà le diagnostic : si tout ce dont le site a besoin se trouve dans le même dossier principal, on sait où chercher.

---

## Slide 13 — Chemin absolu et chemin relatif : première intuition

Un chemin indique où se trouve une ressource.

Un **chemin absolu** décrit un emplacement à partir d'un point de référence global, par exemple une URL complète. Un **chemin relatif** décrit la position d'une ressource par rapport au fichier courant.

Dans vos petits sites, nous utiliserons surtout des chemins relatifs. Si `index.html` et `contact.html` sont dans le même dossier, `contact.html` suffit pour passer de l'un à l'autre.

Cette notion sera reprise lentement avec les liens et les images.

---

## Slide 14 — Pourquoi `images/photo.jpg` a du sens

Si `index.html` se trouve dans le dossier principal et que `photo.jpg` se trouve dans le sous-dossier `images`, le chemin relatif peut être écrit :

```text
images/photo.jpg
```

On peut le lire comme une instruction humaine : « depuis l'endroit où je suis, entre dans le dossier `images`, puis prends `photo.jpg` ».

Comprendre cette phrase vaut mieux que mémoriser une syntaxe sans savoir ce qu'elle signifie.

**Visuel suggéré :** arborescence avec une flèche partant de `index.html` vers `images/photo.jpg`.

---

## Slide 15 — Un éditeur de code n'est pas Word

Un document HTML doit rester un fichier texte contenant exactement les caractères que vous écrivez.

Un traitement de texte comme Word ajoute de la mise en forme, des métadonnées et une structure de document qui ne conviennent pas à l'édition directe de code source.

Nous allons donc utiliser un **éditeur de code**, Visual Studio Code. Il affiche le texte du fichier, colore la syntaxe et fournit des outils utiles pour travailler sur un projet.

---

## Slide 16 — Visual Studio Code

Visual Studio Code, souvent abrégé **VS Code**, est un éditeur de code disponible sur plusieurs systèmes d'exploitation.

Il permet notamment d'ouvrir un dossier de projet, naviguer entre les fichiers, créer et modifier des documents, rechercher dans le code et utiliser de nombreuses extensions.

Cette semaine, nous n'utiliserons qu'une petite partie de ses possibilités. L'objectif n'est pas de maîtriser VS Code, mais de disposer d'un environnement stable pour écrire nos fichiers HTML.

**Visuel suggéré :** interface schématique de VS Code avec Explorateur, éditeur et barre d'état.

---

## Slide 17 — Ouvrir le dossier, pas seulement le fichier

Une bonne habitude consiste à ouvrir **le dossier du projet** dans VS Code plutôt qu'à ouvrir uniquement un fichier isolé.

L'Explorateur de VS Code affiche alors l'ensemble de l'arborescence. Vous voyez immédiatement où se trouvent vos pages et vos images.

Cette pratique réduit les erreurs de chemin et facilite la navigation entre les fichiers.

**Exemple :** si le dossier `images` n'apparaît pas dans votre projet VS Code alors que votre code l'utilise, cela doit immédiatement vous pousser à vérifier votre organisation.

---

## Slide 18 — Créer, modifier… et enregistrer

Une modification effectuée dans l'éditeur n'est pas forcément immédiatement écrite dans le fichier sur le disque. Il faut enregistrer le document.

Le raccourci `Ctrl + S` deviendra rapidement un réflexe.

L'une des premières situations rencontrées par les débutants est : « J'ai modifié mon titre mais le navigateur affiche toujours l'ancien. » Avant de chercher une erreur compliquée, vérifiez simplement que le fichier a été enregistré.

**Anecdote de terrain :** « As-tu enregistré ? » est une question simple, mais extrêmement rentable en dépannage débutant.

---

## Slide 19 — Le navigateur et VS Code ont deux rôles différents

VS Code sert à **modifier les fichiers**. Le navigateur sert à **interpréter et afficher** la page.

Le cycle de travail le plus simple sera donc : modifier dans VS Code → enregistrer → revenir dans le navigateur → actualiser la page → observer le résultat.

Cette boucle très courte sera répétée des dizaines de fois pendant la semaine.

Elle constitue déjà une forme de développement itératif : on effectue une petite modification, on observe, puis on ajuste.

---

## Slide 20 — Prêts pour le premier fichier HTML

Nous savons maintenant qu'une page Web repose sur plusieurs technologies, qu'HTML décrit la structure du contenu, qu'un site utilise des fichiers organisés en dossiers et qu'un éditeur de code permet de modifier ces fichiers proprement.

Nous allons pouvoir créer notre premier `index.html`.

Le point important n'est pas de recopier rapidement un modèle. Chaque ligne sera expliquée : le but est qu'à terme vous sachiez reconstruire la structure d'une page sans copier mécaniquement un bloc incompris.

**Visuel suggéré :** fichier `index.html` vide avec un curseur, comme un point de départ.
