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

## Exercices 41 à 48 — Missions longues

Ces missions ne possèdent volontairement pas de corrigé unique. Avant de valider, contrôler les invariants suivants :

1. toutes les pages et tous les dossiers demandés existent ;
2. la navigation fonctionne depuis la racine comme depuis les sous-dossiers ;
3. chaque page possède un `title`, un `h1` unique et un `main` unique ;
4. les balises imposées sont utilisées pour leur sens, pas seulement pour leur apparence ;
5. toutes les images sont locales, affichées, décrites par un `alt` adapté et créditées ;
6. tableaux et formulaires restent compréhensibles au clavier et sans CSS ;
7. les volumes de contenu demandés sont respectés ;
8. l'étudiant peut montrer un problème rencontré et expliquer sa résolution.

### Points de vigilance particuliers

- **41 — Tintin :** cinq pages, quatre aventures réellement développées, CV distinct du récit des aventures, page Milou, tableau de compétences, formulaire et sources. Ne pas exiger l'utilisation d'images protégées trouvées au hasard : accepter des visuels fournis, des illustrations personnelles ou des images réutilisables et créditées.
- **42 — Sherlock Holmes :** chemins avec `../`, trois affaires, raisonnement visible avant la conclusion et tableaux d'indices cohérents.
- **43 — Musée :** six objets distincts, catalogue structuré, informations de visite, FAQ et formulaire correctement étiqueté.
- **44 — Phileas Fogg :** quatre étapes détaillées, navigation précédent/suivant, tableau d'itinéraire et retours corrects depuis `etapes/`.
- **45 — Festival :** tableau accessible, huit artistes, trois lieux et formulaire structuré en groupes logiques.
- **46 — Phénomènes :** cinq dossiers comparables, métadonnées dans `dl`, hypothèses contradictoires et formulaire utilisable au clavier.
- **47 — Mythologie :** huit créatures, quatre traditions, sources explicites et absence de caricature culturelle.
- **48 — Hypertexte :** quinze scènes, quatre fins, trois objets, deux énigmes, boucle volontaire et aucune impasse accidentelle.

Une mission longue est considérée comme excellente lorsque le site peut être testé sans explication orale préalable, puis que son auteur sait justifier son arborescence, ses chemins relatifs et ses choix sémantiques.

## Grille rapide pour les mini-projets

| Critère | 0 | 1 | 2 |
|---|---:|---:|---:|
| Structure HTML | absente ou cassée | globalement correcte | complète et cohérente |
| Navigation et chemins | plusieurs blocages | un défaut mineur | tout est testé |
| Sémantique | balises surtout choisies pour l'apparence | choix généralement adaptés | choix précis et expliqués |
| Accessibilité de base | titres, `alt` ou labels absents | quelques oublis | essentiels présents |
| Autonomie | ne peut pas expliquer | explique avec aide | explique et diagnostique |

Score indicatif sur 10. Demander à chaque étudiant de montrer un bug résolu et une décision de structure avant de conclure.
