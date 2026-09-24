# Banque de 48 exercices HTML

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

## Niveau 6 — Missions longues pour les plus rapides

Ces missions sont de véritables petits projets. Elles demandent entre **1 h 30 et 3 h** et ne doivent être commencées qu'après validation des fondamentaux. Elles restent réalisables en HTML pur ; le [thème CSS fourni](SUPPORTS/README.md) peut être relié sans être modifié.

### Documentation de référence

Lorsqu'une balise est nouvelle, consultez sa documentation avant de l'utiliser :

- [organiser le contenu avec `main`](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/main), [`nav`](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/nav), [`section`](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/section) et [`article`](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/article) ;
- [associer une image et sa légende avec `figure`](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/figure) et [`figcaption`](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/figcaption) ;
- [représenter une date avec `time`](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/time) et [des coordonnées avec `address`](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/address) ;
- [construire un tableau accessible](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/table) avec une légende et des en-têtes ;
- [construire un formulaire](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/form), [relier les libellés avec `label`](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/label) et [regrouper les champs avec `fieldset`](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/fieldset) ;
- [créer un bloc dépliant avec `details`](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/details) et [`summary`](https://developer.mozilla.org/fr/docs/Web/HTML/Reference/Elements/summary).

Lorsque le site est terminé, vous pouvez soumettre chaque page au [validateur HTML du W3C](https://validator.w3.org/nu/) et corriger les erreurs signalées avant la recette finale.

Les images doivent être enregistrées dans le projet, jamais affichées directement depuis l'adresse d'un autre site. Utilisez des images fournies par l'enseignant, des ressources dont la réutilisation est autorisée ou vos propres illustrations. Ajoutez toujours la source et la licence sur une page `sources.html`.

### Exercice 41 — Le CV extraordinaire de Tintin · 2 h à 3 h · ★★★★

Tintin souhaite quitter provisoirement le journalisme pour postuler comme **reporter d'investigation international**. Votre mission consiste à créer son site de candidature. Il ne s'agit pas d'une page isolée, mais d'un site cohérent donnant envie de découvrir son parcours.

#### Informations à utiliser

- **Profil :** jeune reporter belge, curieux, courageux, observateur, loyal et toujours prêt à défendre les personnes menacées.
- **Compétences :** enquête, entretien de témoins, recherche d'indices, rédaction, photographie, conduite de nombreux véhicules, orientation, diplomatie et sang-froid.
- **Compagnon :** Milou, fox-terrier blanc, fidèle, intelligent, parfois gourmand et souvent décisif dans les moments dangereux.
- **Proches :** le capitaine Haddock, le professeur Tournesol, les détectives Dupond et Dupont et la cantatrice Bianca Castafiore.
- **Expériences à présenter :** enquête à Shanghai dans *Le Lotus bleu* ; recherche maritime dans *Le Secret de La Licorne* et *Le Trésor de Rackham le Rouge* ; préparation puis voyage lunaire dans *Objectif Lune* et *On a marché sur la Lune* ; expédition de secours dans *Tintin au Tibet*.
- **Qualités à illustrer :** persévérance, amitié, curiosité, capacité d'adaptation et sens de la justice.

#### Arborescence obligatoire

```text
cv-tintin/
├── index.html
├── aventures.html
├── milou.html
├── candidature.html
├── sources.html
└── images/
    ├── portrait-tintin.jpg
    ├── milou.jpg
    ├── aventure-lune.jpg
    └── aventure-tibet.jpg
```

Si les fichiers fournis portent une autre extension, adaptez les chemins sans les renommer au hasard.

#### Contenu page par page

- `index.html` présente le CV : titre professionnel, profil, cinq compétences, trois qualités, expériences synthétiques et lien de contact fictif. Utilisez `header`, `nav`, `main`, au moins trois `section`, `figure`, `address` et `footer`.
- `aventures.html` raconte au moins quatre aventures sous forme de quatre `article`. Chaque aventure possède un titre, un résumé de 80 mots minimum, une compétence mobilisée, une image légendée et un lien « retour en haut ».
- `milou.html` présente Milou, son caractère et trois situations dans lesquelles il aide Tintin. Ajoutez une citation fictive clairement signalée comme telle, une liste de qualités et une galerie de deux images minimum.
- `candidature.html` contient une lettre de motivation de 180 mots minimum, un tableau associant cinq missions à cinq compétences et un formulaire fictif permettant de proposer une nouvelle mission. Le formulaire ne sera pas réellement envoyé.
- `sources.html` crédite chaque image : titre ou description, auteur si connu, site d'origine, lien et conditions de réutilisation.

#### Contraintes globales

La même navigation apparaît sur les cinq pages. Chaque page possède un `title` différent, un seul `h1` et une hiérarchie de titres régulière. Les quatre images sont obligatoires, locales et accompagnées d'un `alt` utile. Les titres d'œuvres utilisent `cite`. Les liens ne doivent jamais être intitulés « cliquez ici ».

**Validation :** partez successivement de chacune des cinq pages et testez toute la navigation. Retirez ensuite le CSS : le site doit conserver son sens, son ordre de lecture et toutes ses informations.

**Extension expert :** ajoutez `chronologie.html` avec un tableau chronologique, un sommaire d'ancres et une rubrique dépliante « Ce que cette aventure m'a appris » pour chaque mission.

### Exercice 42 — Les archives de Sherlock Holmes · 2 h à 3 h · ★★★★

Le docteur Watson veut numériser les dossiers du 221B Baker Street. Créez un site de cinq pages : accueil, trois affaires et index des indices. Les affaires peuvent être inspirées de récits connus ou entièrement inventées, mais elles doivent rester cohérentes.

**Arborescence minimale :** `index.html`, `affaires/ruban.html`, `affaires/horloge.html`, `affaires/empreinte.html`, `indices.html`, `images/` et `sources.html`. Cette structure vous oblige à maîtriser les chemins utilisant `../`.

Chaque affaire contient un `article`, une date avec `time`, une liste de suspects, un tableau « indice / observation / déduction », un témoignage dans `blockquote`, deux figures et une conclusion rangée dans `details`. L'accueil présente Holmes, Watson et une navigation vers tous les dossiers. L'index classe au moins douze indices par affaire.

**Images obligatoires :** portrait ou silhouette, plan d'un lieu, objet mystérieux et indice matériel. Elles doivent être locales, légendées et créditées.

**Validation :** le lecteur doit pouvoir résoudre chaque affaire avant d'ouvrir la conclusion. Vérifiez tous les liens depuis une page située dans `affaires`.

**Extension expert :** écrivez une quatrième affaire dont la conclusion dépend du croisement d'au moins trois indices dispersés sur différentes pages.

### Exercice 43 — Le musée des inventions impossibles · 2 h · ★★★★

Concevez le site d'un musée exposant au moins six objets absurdes : parapluie à l'envers, grille-pain temporel, traducteur de miaulements ou inventions personnelles.

Créez un accueil, une page `collection.html`, deux pages détaillées d'œuvre, une page `visite.html` et `sources.html`. La collection utilise six `article`. Chaque objet possède un nom, un inventeur, une date avec `time`, une fonction, un danger, une figure légendée et un numéro d'inventaire. La page de visite contient les coordonnées dans `address`, un tableau d'horaires et tarifs, une FAQ avec quatre couples `details`/`summary`, puis un formulaire de réservation comprenant `label`, `fieldset` et `legend`.

**Images obligatoires :** une image par invention. Vous pouvez réaliser des dessins simples, des photomontages personnels ou utiliser des images réutilisables correctement créditées.

**Validation :** la collection doit être compréhensible comme catalogue, le tableau ne doit pas servir à la mise en page et tous les libellés du formulaire doivent être cliquables.

**Extension expert :** ajoutez une page « exposition temporaire » et un tableau comparant danger, utilité et rareté des six objets.

### Exercice 44 — Le tour du monde de Phileas Fogg · 2 h à 3 h · ★★★★

Racontez un itinéraire inspiré du *Tour du monde en quatre-vingts jours*. Le site doit fonctionner à la fois comme carnet de voyage et comme dossier logistique.

Créez `index.html`, `itineraire.html`, `etapes/londres.html`, `etapes/bombay.html`, `etapes/yokohama.html`, `etapes/new-york.html`, `compagnons.html` et `sources.html`. L'itinéraire contient un tableau avec lieu, moyen de transport, durée prévue, incident et retard. Chaque étape comporte un `article` d'au moins 120 mots, une date structurée, une figure, une liste de préparatifs et un lien vers l'étape suivante et la précédente. La page des compagnons présente Phileas Fogg, Passepartout, Fix et Aouda.

**Images obligatoires :** portrait ou silhouette de quatre personnages, quatre villes et au moins trois moyens de transport. Une même image pertinente peut apparaître sur plusieurs pages, mais elle n'est comptée qu'une fois.

**Validation :** suivez tout le voyage sans employer le bouton « précédent » du navigateur. Depuis chaque sous-dossier, le retour à l'accueil doit fonctionner.

**Extension expert :** ajoutez deux itinéraires alternatifs et comparez durée, risque et coût dans un second tableau.

### Exercice 45 — Le festival intergalactique · 2 h · ★★★★

Une station spatiale organise trois jours de concerts pour des espèces venues de cinq planètes. Réalisez le site public complet de l'évènement.

Le site contient au minimum les pages accueil, programme, artistes, lieux, inscription et informations pratiques. Le programme utilise `caption`, `thead`, `tbody`, `th scope="col"` et `th scope="row"`. La page artistes présente au moins huit groupes dans des `article`, avec planète d'origine, style musical, horaire, biographie et image. La page lieux propose trois salles avec capacité et consignes. Le formulaire d'inscription recueille identité, planète, jour choisi, besoins alimentaires et autorisation de recevoir des nouvelles.

**Images obligatoires :** logo original du festival, huit artistes ou groupes et trois lieux. Toutes les images doivent avoir un rôle compréhensible et un texte alternatif adapté.

**Validation :** une personne découvrant le festival doit trouver en moins d'une minute qui joue, où, quand et comment s'inscrire.

**Extension expert :** construisez une page imprimable « mon programme » contenant une sélection cohérente sans chevauchement d'horaires.

### Exercice 46 — Le bureau des phénomènes impossibles · 2 h 30 · ★★★★

Vous êtes archiviste dans une administration enquêtant sur des phénomènes que la science ne sait pas encore expliquer. Produisez un portail comprenant un tableau de bord, cinq dossiers, un registre des témoins et un formulaire de signalement.

Chaque dossier possède un identifiant, un lieu, une date, un niveau de danger, un statut, deux témoignages, trois indices, deux hypothèses contradictoires et une conclusion provisoire. Structurez chaque dossier dans `article`, les témoignages dans `blockquote`, les métadonnées dans une liste de descriptions `dl`, et les hypothèses dans deux `section`. Le tableau de bord compare les cinq affaires dans un tableau. Le formulaire de signalement regroupe coordonnées, localisation, date, description et niveau d'urgence dans plusieurs `fieldset`.

**Images obligatoires :** au moins huit pièces visuelles locales réparties entre dossiers, avec légendes et sources.

**Validation :** chaque dossier doit pouvoir être lu indépendamment, mais rester accessible depuis le registre général. Le formulaire doit être entièrement utilisable au clavier.

**Extension expert :** dissimulez un lien logique entre les cinq dossiers grâce à des indices textuels cohérents, puis créez une page secrète accessible seulement après déduction de son nom de fichier.

### Exercice 47 — Encyclopédie des créatures mythologiques · 2 h 30 · ★★★★

Créez une encyclopédie structurée consacrée à huit créatures issues d'au moins quatre traditions culturelles différentes. Le but n'est pas d'accumuler des images, mais d'organiser et de comparer une information riche.

Prévoyez une page d'accueil, une page par grande région, au moins quatre fiches détaillées, un comparateur et une bibliographie. Chaque fiche indique nom, origine, apparence, habitat, comportement, récit célèbre et niveau de danger. Utilisez `article`, `section`, `dl`, `figure`, `figcaption`, `cite` et des liens d'ancres. Le comparateur présente les huit créatures dans un tableau accessible. La bibliographie distingue livres, musées et ressources Web.

**Images obligatoires :** huit illustrations locales et créditées. N'utilisez pas la nationalité ou la culture comme une caricature : décrivez les récits et indiquez vos sources.

**Validation :** un lecteur doit pouvoir naviguer par région, par créature et revenir au comparateur depuis chaque fiche.

**Extension expert :** ajoutez un questionnaire HTML sans JavaScript permettant au visiteur de noter sur papier la créature qui correspond le mieux à ses réponses.

### Exercice 48 — Grande aventure hypertexte · 3 h et plus · ★★★★★

Créez un livre-jeu complet en HTML pur. Le lecteur explore un lieu inquiétant ou merveilleux en cliquant sur ses décisions. Aucun JavaScript n'est autorisé : l'état de l'histoire est représenté par des pages différentes.

Le projet contient au moins quinze pages de scène, quatre fins, trois objets, deux énigmes, une boucle volontaire et une page `carte-auteur.html` qui explique tous les chemins. Chaque scène présente un titre, un texte de 100 mots minimum, une image locale, deux choix significatifs et un lien pour recommencer. Pour simuler un objet, créez par exemple `grotte-sans-cle.html` et `grotte-avec-cle.html` : le texte et les choix changent selon le chemin suivi.

L'une des énigmes doit demander de réunir des informations trouvées sur trois pages. Une mauvaise réponse peut renvoyer vers une boucle, mais jamais vers une véritable page morte. Les quatre fins doivent être réellement différentes : réussite, échec, abandon et fin secrète.

**Images obligatoires :** au moins dix illustrations locales, dont une carte, trois objets et quatre lieux. Les textes alternatifs ne doivent pas révéler la solution d'une énigme.

**Validation :** faites tester l'histoire par un camarade sans lui parler. Notez son parcours, les impasses involontaires et les choix ambigus, puis corrigez-les.

**Extension expert :** concevez deux versions d'une même zone selon la possession de deux objets différents, ce qui porte le projet à vingt pages ou davantage.

## Règle de fin d'exercice

Avant d'annoncer « terminé » :

1. rechargez la page ;
2. testez chaque lien et chaque image ;
3. ouvrez les outils de développement ou le validateur indiqué par l'enseignant ;
4. relisez le code et son indentation ;
5. préparez une phrase expliquant ce que vous avez appris.
