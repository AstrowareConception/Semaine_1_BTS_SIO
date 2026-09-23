# Banque de 40 exercices HTML

Les exercices sont indépendants sauf indication contraire. Créez un dossier par exercice : `ex01`, `ex02`, etc. Testez chaque page dans le navigateur avant de passer à la suivante.

Le CSS n'est jamais obligatoire. Pour un rendu plus agréable, vous pouvez relier le fichier [`theme-fourni.css`](SUPPORTS/theme-fourni.css) sans le modifier.

## Niveau 1 — Prise en main

### Exercice 1 — La toute première page · 10 min · ★

Créez `index.html` avec le squelette complet, un titre d'onglet, un `h1` et deux paragraphes. Le navigateur doit afficher les accents correctement.

**Validation :** le titre de l'onglet et le grand titre sont différents ; aucune balise visible à l'écran.

### Exercice 2 — Une hiérarchie claire · 10 min · ★

Présentez un animal imaginaire avec un `h1`, deux parties en `h2` et deux sous-parties en `h3`. N'utilisez pas un niveau de titre uniquement pour sa taille.

**Validation :** on comprend le plan en ne lisant que les titres.

### Exercice 3 — Mettre du sens dans le texte · 10 min · ★

Écrivez une annonce contenant une information importante avec `strong`, un mot sur lequel insister avec `em` et une abréviation expliquée avec `abbr`.

**Validation :** vous savez expliquer la différence entre importance et apparence.

### Exercice 4 — Inventaire ou procédure ? · 10 min · ★

Créez une liste non ordonnée de cinq objets à emporter, puis une liste ordonnée de cinq étapes à suivre.

**Validation :** inverser l'ordre de la première liste ne change pas son sens ; inverser la seconde le change.

### Exercice 5 — Liste à étages · 15 min · ★★

Créez la carte d'un restaurant fictif : trois catégories et, dans chacune, au moins trois plats. Imbriquez correctement les listes.

**Validation :** chaque sous-liste est placée à l'intérieur du `li` auquel elle appartient.

### Exercice 6 — Sortie vers le Web · 10 min · ★

Ajoutez deux liens externes utiles. Le texte des liens doit annoncer leur destination sans employer « cliquez ici ».

**Validation :** les deux liens fonctionnent et commencent par `https://`.

### Exercice 7 — Une image locale · 15 min · ★

Créez un dossier `images`, placez-y une image, affichez-la et rédigez un `alt` utile. Si l'image est purement décorative, utilisez un `alt` vide et expliquez pourquoi.

**Validation :** renommez temporairement l'image : l'absence du fichier doit révéler un texte alternatif pertinent.

### Exercice 8 — Image et légende · 15 min · ★★

Présentez une invention absurde avec `figure`, `img` et `figcaption`.

**Validation :** la légende décrit le rôle de l'image ; le `alt` n'en est pas une copie mécanique.

### Exercice 9 — Commentaires utiles · 10 min · ★

Ajoutez trois commentaires HTML : début d'une grande partie, rappel à terminer et explication d'un choix inhabituel.

**Validation :** ils sont visibles dans le code source, jamais dans la page.

### Exercice 10 — Montrer du code · 15 min · ★★

Affichez un petit exemple HTML à l'intérieur de `pre` et `code`. Faites apparaître les caractères `<` et `>` sans que le navigateur interprète l'exemple.

**Indice :** cherchez les entités `&lt;` et `&gt;`.

## Niveau 2 — Structurer et naviguer

### Exercice 11 — Page sémantique · 20 min · ★★

Transformez une page simple afin qu'elle utilise `header`, `nav`, `main`, au moins une `section` et `footer`.

**Validation :** chaque zone a une fonction claire et `main` n'apparaît qu'une fois.

### Exercice 12 — Le mini-site trois pages · 30 min · ★★

Créez `index.html`, `galerie.html` et `contact.html`. Chaque page possède la même navigation et permet de revenir à l'accueil.

**Validation :** testez tous les liens depuis chacune des trois pages.

### Exercice 13 — Sommaire express · 20 min · ★★

Créez une longue page avec quatre sections identifiées par des `id`. Ajoutez en haut un sommaire d'ancres internes et, après chaque section, un retour vers le sommaire.

**Validation :** l'URL change après un clic et aucun lien n'arrive au mauvais endroit.

### Exercice 14 — FAQ dépliante · 15 min · ★★

Créez cinq questions-réponses avec `details` et `summary`. Une réponse contient une liste et une autre un lien externe.

**Validation :** les réponses restent compréhensibles sans CSS ni JavaScript.

### Exercice 15 — Mini-glossaire · 15 min · ★★

Expliquez cinq mots du Web avec `dl`, `dt` et `dd` : navigateur, serveur, URL, balise et attribut.

**Validation :** chaque terme est suivi de sa définition et non présenté comme une simple liste à puces.

### Exercice 16 — La citation mystérieuse · 15 min · ★★

Présentez une citation longue avec `blockquote`, sa source avec `cite`, puis une courte réaction personnelle.

**Validation :** les mots de la source ne sont pas mélangés avec votre commentaire.

### Exercice 17 — Une vraie fiche contact · 20 min · ★★

Créez une fiche comprenant un `address`, un lien `mailto:`, un lien `tel:` et deux horaires représentés par `time`.

**Validation :** les liens utilisent les bons protocoles et le contenu reste lisible sur papier.

### Exercice 18 — Article de presse extraterrestre · 25 min · ★★

Rédigez une actualité fictive dans `article` : titre, date, auteur, introduction, deux sections et source.

**Validation :** l'article pourrait être réutilisé seul sans perdre son sens.

## Niveau 3 — Tableaux et formulaires

### Exercice 19 — Tableau de scores · 20 min · ★★

Créez un tableau de quatre joueurs avec nom, équipe et score. Utilisez une ligne d'en-têtes.

**Validation :** les données sont réellement tabulaires ; elles ne servent pas à placer la page.

### Exercice 20 — Comparatif complet · 30 min · ★★★

Comparez quatre créatures ou produits avec `caption`, `thead`, `tbody`, `th` et `td`. Chaque ligne doit avoir un en-tête.

**Validation :** la légende annonce ce que l'on compare et les en-têtes permettent de lire chaque valeur.

### Exercice 21 — Emploi du temps · 35 min · ★★★

Représentez une demi-journée de cours dans un tableau. Utilisez `colspan` ou `rowspan` au moins une fois, sans casser l'alignement.

**Validation :** chaque ligne possède le bon nombre logique de cellules.

### Exercice 22 — Contact minimal · 25 min · ★★

Créez un formulaire avec nom, e-mail, sujet, message et bouton d'envoi. Chaque champ possède un `label` relié par `for` et `id`.

**Validation :** cliquer sur un libellé place le curseur dans son champ.

### Exercice 23 — Inscription au club · 35 min · ★★★

Ajoutez prénom, nom, e-mail, date de naissance, mot de passe et choix d'activité. Employez des types de champs adaptés et `required` lorsque nécessaire.

**Validation :** le navigateur bloque un envoi vide et détecte un e-mail manifestement incorrect.

### Exercice 24 — Sondage loufoque · 30 min · ★★★

Demandez une seule « planète préférée » avec des boutons radio, puis plusieurs « pouvoirs souhaités » avec des cases à cocher.

**Validation :** un seul bouton radio peut rester sélectionné ; plusieurs cases peuvent l'être.

### Exercice 25 — Le videur du formulaire · 25 min · ★★★

Créez un pseudonyme de 3 à 20 caractères, un âge de 16 à 99 et une adresse e-mail obligatoire. Utilisez les attributs de validation HTML adaptés.

**Validation :** essayez volontairement cinq valeurs invalides et notez les réactions du navigateur.

### Exercice 26 — Formulaire bien rangé · 30 min · ★★★

Répartissez un formulaire en deux `fieldset` : identité et préférences. Donnez à chacun une `legend` claire.

**Validation :** même sans CSS, les deux groupes sont visuellement et sémantiquement distincts.

### Exercice 27 — Mission en progression · 20 min · ★★★

Créez une fiche de mission avec une barre `progress` pour l'avancement et deux jauges `meter` pour l'énergie et le niveau de danger.

**Validation :** vous pouvez expliquer pourquoi `progress` et `meter` ne représentent pas la même chose.

### Exercice 28 — Audit d'accessibilité · 30 min · ★★★

Choisissez une page déjà créée. Vérifiez : langue du document, titre d'onglet, ordre des titres, textes alternatifs, textes de liens, libellés de formulaire et navigation au clavier. Corrigez au moins cinq points et ajoutez un commentaire listant vos corrections.

**Validation :** la page demeure compréhensible lorsque le CSS fourni est retiré.

## Niveau 4 — Déboguer

Les fichiers de départ se trouvent dans [`ATELIERS_DEBUG`](ATELIERS_DEBUG/README.md). Avant toute modification, écrivez votre diagnostic en une phrase.

### Exercice 29 — Balises en fuite · 15 min · ★★

Réparez l'atelier 1 : balises fermées au mauvais endroit, titres incohérents et éléments manquants.

### Exercice 30 — Poupées russes · 15 min · ★★

Réparez l'atelier 2 : imbrications impossibles et liste mal construite.

### Exercice 31 — L'image fantôme · 20 min · ★★

Réparez l'atelier 3 sans déplacer l'image. Expliquez le chemin relatif correct.

### Exercice 32 — Labyrinthe de liens · 25 min · ★★★

Réparez l'atelier 4 : navigation entre un fichier racine et un fichier placé dans `pages`.

### Exercice 33 — Tableau et formulaire accidentés · 30 min · ★★★

Réparez l'atelier 5, puis testez les libellés et la structure du tableau.

### Exercice 34 — Sauvetage global · 40 min · ★★★

Réparez l'atelier 6 sans repartir de zéro. Faites d'abord une liste de toutes les erreurs, puis corrigez-les une par une.

## Niveau 5 — Défis créatifs

### Exercice 35 — Recette impossible · 30 min · ★★

Inventez une recette absurde avec ingrédients, étapes, durée, avertissement, figure et légende. Le contenu est loufoque ; la structure doit être irréprochable.

### Exercice 36 — Carte de créature numérique · 30 min · ★★

Présentez le Dévoreur de RAM, le Spectre 404 ou votre propre créature avec une fiche d'identité, une figure, des caractéristiques et une citation.

### Exercice 37 — Musée d'un objet banal · 35 min · ★★★

Créez la page d'exposition solennelle d'une chaussette, d'une agrafeuse ou d'un autre objet banal : cartel, histoire, figure, citation de conservateur et informations de visite.

### Exercice 38 — Micro-aventure hypertexte · 45 min · ★★★

Créez au moins six pages reliées par des choix. Prévoyez deux fins et un moyen de recommencer. Aucun JavaScript.

**Validation :** aucune page ne doit laisser le lecteur bloqué involontairement.

### Exercice 39 — CV d'un personnage fictif · 40 min · ★★★

Réalisez le CV de Batman, d'un robot stagiaire ou d'un dragon administrateur réseau : profil, expériences, compétences, langues, loisirs et contact.

**Validation :** utilisez des titres cohérents et des dates structurées ; n'inventez pas de vraies coordonnées personnelles.

### Exercice 40 — Guide de décision · 45 min · ★★★

Créez un guide aidant à choisir entre quatre destinations, métiers imaginaires ou animaux de compagnie fantastiques. Combinez sommaire, fiches, tableau comparatif et conclusion argumentée.

**Validation :** un lecteur doit pouvoir prendre une décision en moins de deux minutes.

## Règle de fin d'exercice

Avant d'annoncer « terminé » :

1. rechargez la page ;
2. testez chaque lien et chaque image ;
3. ouvrez les outils de développement ou le validateur indiqué par l'enseignant ;
4. relisez le code et son indentation ;
5. préparez une phrase expliquant ce que vous avez appris.
