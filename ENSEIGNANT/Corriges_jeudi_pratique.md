# Repères de correction — jeudi de pratique HTML

Ce document donne des critères et des pistes. Plusieurs productions peuvent être correctes : on évalue d'abord la structure, le sens, les chemins et la capacité à expliquer.

## Exercices 1 à 10 — Fondamentaux

| Exercice | Points attendus |
|---|---|
| 1 | `doctype`, `html lang="fr"`, `head`, `meta charset`, `title`, `body`, `h1`, deux `p` |
| 2 | un seul `h1`, niveaux non sautés, titres décrivant le plan |
| 3 | `strong` pour l'importance, `em` pour l'emphase, `abbr title` pour l'expansion |
| 4 | `ul` pour l'inventaire, `ol` pour la procédure |
| 5 | la sous-liste est enfant du `li` de catégorie |
| 6 | URL absolues en `https://`, textes de liens explicites |
| 7 | fichier dans `images`, chemin relatif exact, `alt` adapté à la fonction |
| 8 | `img` et `figcaption` contenus dans `figure` |
| 9 | syntaxe `<!-- commentaire -->`, commentaires utiles et invisibles |
| 10 | `pre > code`, chevrons échappés avec `&lt;` et `&gt;` |

## Exercices 11 à 18 — Structure et navigation

- 11 : `header`, `nav`, un seul `main`, sections titrées et `footer`.
- 12 : chemins relatifs corrects dans les deux sens ; navigation répétée et cohérente.
- 13 : identifiants uniques, liens de la forme `href="#identifiant"` et retour au sommaire.
- 14 : chaque `summary` est le premier enfant de son `details`.
- 15 : groupes `dt`/`dd` à l'intérieur de `dl`.
- 16 : citation dans `blockquote`, source distincte avec `cite`.
- 17 : `address`, `mailto:`, `tel:` et `time datetime` avec valeurs exploitables.
- 18 : article autonome, date, auteur, titre principal et sections cohérentes.

## Exercices 19 à 28 — Données, formulaires, accessibilité

- 19 : une ligne d'en-têtes, trois colonnes constantes et quatre lignes de données.
- 20 : `caption`, `thead`, `tbody` ; `th scope="col"` et idéalement `th scope="row"`.
- 21 : cellules fusionnées comptées correctement ; les en-têtes restent compréhensibles.
- 22 : chaque `label for` correspond exactement à un `input id` ou `textarea id`.
- 23 : types `text`, `email`, `date`, `password` ; attributs `name` et `required` pertinents.
- 24 : même `name` pour les radios d'un groupe ; noms et valeurs utiles pour les cases.
- 25 : `minlength="3"`, `maxlength="20"`, `type="number" min="16" max="99"`, `type="email" required`.
- 26 : deux groupes `fieldset` avec chacun une `legend`.
- 27 : `progress` représente l'avancement ; `meter` une mesure dans un intervalle connu.
- 28 : au moins cinq corrections réelles, justifiables et vérifiées au clavier.

## Corrigé des ateliers de débogage

### 29 — Balises en fuite

- fermer `h1` avec `</h1>` ;
- fermer le paragraphe avec `</p>` ;
- remplacer le `h3` par un `h2` et fermer avec `</h2>` ;
- fermer le premier `li` ;
- fermer la liste avec `</ul>`.

### 30 — Poupées russes

- placer `</strong>` avant `</p>` ;
- déplacer chaque sous-liste à l'intérieur du `li` correspondant ;
- fermer la liste ordonnée avec `</ol>` ;
- vérifier la fermeture de tous les `li`.

### 31 — L'image fantôme

Le fichier HTML se trouve à côté du dossier `images`. Le bon chemin est `images/robot.svg`.

### 32 — Labyrinthe de liens

- accueil vers profil : `pages/profil.html` ;
- profil vers accueil : `../index.html`.

### 33 — Tableau et formulaire accidentés

- donner le même nombre logique de cellules aux lignes ;
- décider si « Bonus secret » devient une vraie troisième colonne ou doit disparaître ;
- ajouter la valeur manquante sur la dernière ligne ;
- faire correspondre `for="nom"` à `id="nom"` ;
- ajouter un `label for="email"`, `id="email"` et `type="email"`.

### 34 — Sauvetage global

Erreurs principales : balise `title` mal fermée, `lang` et `meta charset` absents, niveaux de titres mal fermés, lien `index.htm`, ancre `#offre` différente de `id="offres"`, image inexistante et sans `alt`, `strong` mal imbriqué, liste fermée par `ol`, `li` manquant, `label` différent de l'`id`, `main` et `p` mal fermés, balise `html` finale absente.

Pour l'image inexistante, deux réponses sont acceptables : ajouter une vraie ressource dans `images` et corriger le chemin, ou retirer proprement l'image en expliquant le choix.

## Exercices 35 à 40 — Critères communs

Valider si le défi respecte toutes ses contraintes, fonctionne sans CSS, emploie des balises adaptées au sens et peut être expliqué. La créativité ne compense pas une navigation cassée, mais une apparence rudimentaire ne pénalise jamais un HTML solide.

## Grille rapide pour les mini-projets

| Critère | 0 | 1 | 2 |
|---|---:|---:|---:|
| Structure HTML | absente ou cassée | globalement correcte | complète et cohérente |
| Navigation et chemins | plusieurs blocages | un défaut mineur | tout est testé |
| Sémantique | balises surtout choisies pour l'apparence | choix généralement adaptés | choix précis et expliqués |
| Accessibilité de base | titres, `alt` ou labels absents | quelques oublis | essentiels présents |
| Autonomie | ne peut pas expliquer | explique avec aide | explique et diagnostique |

Score indicatif sur 10. Demander à chaque étudiant de montrer un bug résolu et une décision de structure avant de conclure.
