# Je suis bloqué : que faire ?

Être bloqué fait partie du travail informatique. L'objectif n'est pas de ne jamais rencontrer de problème, mais d'apprendre à le décrire et à le rechercher méthodiquement.

# Étape 1 — Décrire précisément le problème

Évitez :

> « Ça marche pas. »

Préférez :

> « Mon fichier `index.html` s'ouvre mais l'image `ordinateur.jpg` n'apparaît pas. »

ou :

> « Quand je clique sur Formation, le navigateur ne trouve pas `formation.html`. »

Une description précise vous aide déjà à réfléchir.

---

# Étape 2 — Vérifier l'évidence

Avant toute chose :

- avez-vous enregistré avec `Ctrl + S` ?
- regardez-vous le bon fichier dans le navigateur ?
- VS Code a-t-il ouvert le bon dossier ?
- le fichier existe-t-il réellement ?
- son extension est-elle correcte ?

---

# Étape 3 — Pour un lien qui ne fonctionne pas

Si vous avez :

```html
<a href="formation.html">Formation</a>
```

vérifiez :

- existe-t-il réellement un fichier `formation.html` ?
- se trouve-t-il dans le même dossier ?
- avez-vous écrit exactement le même nom ?
- avez-vous accidentellement créé `formation.html.txt` ?

---

# Étape 4 — Pour une image absente

Si vous avez :

```html
<img src="images/photo.jpg" alt="Photo">
```

vérifiez que l'arborescence ressemble réellement à :

```text
site/
├── index.html
└── images/
    └── photo.jpg
```

Vérifiez également le nom et l'extension : `photo.jpg` n'est pas forcément `photo.png`.

---

# Étape 5 — Pour du HTML étrange

Inspectez la zone concernée :

- une balise fermante manque-t-elle ?
- un `>` a-t-il été oublié ?
- un guillemet manque-t-il dans un attribut ?
- avez-vous imbriqué les éléments de manière incohérente ?

Ne modifiez qu'une chose à la fois puis testez.

---

# Étape 6 — Demander de l'aide efficacement

Lorsque vous appelez l'enseignant ou un camarade, soyez prêt à montrer :

1. ce que vous vouliez obtenir ;
2. ce que vous obtenez réellement ;
3. le fichier concerné ;
4. l'arborescence de votre dossier ;
5. ce que vous avez déjà vérifié.

Cette méthode fera gagner du temps à tout le monde.

---

# Règle d'entraide

Si vous aidez un camarade, essayez de **ne pas prendre son clavier**.

Posez plutôt des questions :

- « Où est ton fichier ? »
- « Comment s'appelle-t-il exactement ? »
- « Depuis quel fichier pars-tu ? »
- « Où se trouve l'image ? »
- « Ton fichier est-il enregistré ? »

Le but est qu'il sache résoudre un problème similaire la prochaine fois.