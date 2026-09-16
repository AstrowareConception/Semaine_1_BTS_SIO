# Installer et préparer Visual Studio Code

## 1. Avant de commencer

Visual Studio Code — souvent abrégé **VS Code** — est un éditeur de code.

Il ne « crée » pas le site à votre place. Il vous aide à écrire et organiser des fichiers contenant du code.

---

## 2. Créer votre dossier de travail

Créez dans un emplacement que vous retrouverez facilement un dossier :

```text
BTS_SIO
```

À l'intérieur, créez :

```text
Semaine_1
```

Puis :

```text
jour_2_html
```

Vous devez donc obtenir quelque chose de proche de :

```text
BTS_SIO/
└── Semaine_1/
    └── jour_2_html/
```

Cette organisation peut sembler très simple. Elle est volontaire : apprendre à ranger son travail fait partie des premiers réflexes professionnels.

---

## 3. Installer Visual Studio Code

Suivez les indications de l'enseignant pour télécharger et installer VS Code depuis la source officielle.

Pendant cette semaine, nous évitons d'ajouter une grande quantité d'extensions. Un environnement simple est plus facile à comprendre et à dépanner.

---

## 4. Ouvrir un dossier, pas seulement un fichier

Dans VS Code :

1. choisissez **Fichier > Ouvrir un dossier** ;
2. sélectionnez `jour_2_html` ;
3. vérifiez que ce dossier apparaît dans l'explorateur situé à gauche.

Pourquoi ouvrir le dossier complet ? Parce qu'un projet Web contient rapidement plusieurs fichiers et sous-dossiers.

---

## 5. Créer `index.html`

Dans l'explorateur de VS Code :

1. créez un nouveau fichier ;
2. nommez-le exactement :

```text
index.html
```

Attention :

- pas `index.html.txt` ;
- pas `index` ;
- pas `Index.HTML` pour nos exercices ;
- pas d'espace ajouté par erreur.

---

## 6. Enregistrer

Utilisez régulièrement :

```text
Ctrl + S
```

Un fichier modifié mais non enregistré peut expliquer pourquoi votre navigateur n'affiche pas vos derniers changements.

---

## 7. Afficher la page dans le navigateur

Pour l'instant, le fichier peut être ouvert directement avec le navigateur selon les indications données en classe.

Nous ne mettons pas encore en place de serveur Web complet. Notre objectif est d'apprendre HTML.

---

# Les fichiers et leurs extensions

Quelques exemples :

```text
index.html
photo.jpg
logo.png
notes.txt
```

La partie située après le dernier point correspond généralement à l'extension.

Cette extension donne une indication sur le type de contenu.

---

# Les dossiers

Un site pourra bientôt ressembler à :

```text
mon-site/
├── index.html
├── contact.html
└── images/
    ├── logo.png
    └── photo.jpg
```

Prenez l'habitude de lire ce type d'arborescence. Elle indique où se trouve chaque ressource.