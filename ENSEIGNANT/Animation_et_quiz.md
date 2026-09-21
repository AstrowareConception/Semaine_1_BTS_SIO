# Guide enseignant — Animation et quiz

Ce document complète les supports étudiants. Il propose des activités sociales et des questions courtes sans modifier la progression débutante du groupe.

# Principes d'animation

Avec plus de vingt étudiants et des niveaux très disparates :

- annoncer explicitement que le cours principal suit le rythme des débutants ;
- donner des challenges aux étudiants rapides sans transformer ces challenges en prérequis ;
- prévoir régulièrement des plages de 30 à 60 minutes sans nouvelle notion afin de circuler ;
- faire verbaliser les blocages ;
- encourager l'entraide sans prise de contrôle du clavier ;
- utiliser des binômes variables afin d'éviter que les mêmes étudiants deviennent constamment « techniciens de secours ».

---

# Lundi — Quiz diagnostic possible

Support complet :

- [Questions, activités et corrections à projeter](../JOUR_1_LUNDI/SUPPORTS/Support_projection_activites_lundi.pptx)
- diapositives 3 à 25 pour le diagnostic ;
- réponses détaillées dans les notes du présentateur.

Questions Wooclap/Kahoot :

1. Internet et le Web sont exactement la même chose. Vrai/Faux.
2. Lequel est un navigateur ? Chrome / Google / HTML / DNS.
3. À quoi sert principalement DNS dans notre modèle simplifié ?
4. Un serveur Web reçoit des requêtes. Vrai/Faux.
5. Le code 404 signifie-t-il automatiquement qu'Internet est coupé ?
6. Une adresse comme `https://exemple.fr/page.html` est une URL. Vrai/Faux.
7. HTML est-il un navigateur ?
8. Un smartphone peut-il être un client d'un service Internet ?

Ne pas commenter la « note ». Utiliser les réponses pour ajuster les explications.

---

# Icebreaker — Bingo humain projeté

Support prêt à projeter :

- [Bingo humain projeté — 90 affirmations](../JOUR_1_LUNDI/SUPPORTS/Bingo_humain_projete_90_affirmations.pptx)

## Objectifs

- faire circuler rapidement les prénoms ;
- provoquer des échanges légers dès le début de la semaine ;
- révéler la diversité des expériences sans réduire le groupe à son niveau informatique ;
- installer le droit à l'erreur et le réflexe de relais.

## Déroulement conseillé — 55 minutes

1. Projeter une affirmation.
2. Désigner l'étudiant dont c'est le tour ; il propose un prénom.
3. La personne citée confirme ou dément, sans devoir raconter sa vie.
4. Si l'étudiant hésite, ne sait pas ou se trompe, le suivant prend le relais sur la même affirmation.
5. Si la correspondance prête à discussion, organiser un vote rapide à main levée.
6. Passer aussitôt à la diapositive suivante dès qu'une correspondance est confirmée.

Effectuer trois passages par étudiant. Avec 25 étudiants, cela représente 75 prises de parole ; les 15 affirmations supplémentaires permettent de remplacer une proposition inadaptée au groupe ou de prolonger l'activité si le rythme est rapide.

## Règles d'animation

- annoncer explicitement le droit de passer ;
- limiter les commentaires afin de conserver le rythme ;
- accepter une réponse inattendue si la personne citée la confirme ;
- ne pas transformer les affirmations numériques en évaluation ;
- écarter immédiatement une affirmation qui mettrait un étudiant mal à l'aise ;
- utiliser les votes comme un ressort ludique, jamais comme un jugement sur une personne.

Objectif : interaction et découverte du groupe, pas compétition.

---

# Lundi — Web humain

Matériel :

- [cartes de rôles, messages et scénarios à imprimer](../JOUR_1_LUNDI/SUPPORTS/Cartes_Web_humain.pdf) ;
- diapositives 69 à 81 du [support complet des activités](../JOUR_1_LUNDI/SUPPORTS/Support_projection_activites_lundi.pptx).

Huit étudiants deviennent acteurs :

- utilisateur ;
- navigateur ou client ;
- DNS ;
- box ou routeur ;
- Internet ;
- serveur Web ;
- ressource ou page ;
- observateur du protocole.

Les autres étudiants forment des équipes de trois ou quatre enquêteurs. Après chaque scénario, chaque équipe remet un diagnostic comportant :

1. le dernier rôle atteint par le message ;
2. le code ou l'erreur observée ;
3. une phrase expliquant la cause.

Faire circuler des cartes « requête » et « réponse ».

Scénarios :

1. succès — 200 ;
2. fichier absent — 404 ;
3. erreur serveur — 500 ;
4. échec de résolution de nom.

Changer les acteurs après deux scénarios. Les premiers acteurs rejoignent alors les enquêteurs. Attribuer un point par élément correct, sans transformer le résultat en note.

Rester sur le modèle simplifié et préciser qu'il existe de nombreuses étapes supplémentaires dans un échange réel. La réussite du jeu repose sur la qualité du diagnostic, pas sur la vitesse.

---

# Mardi — Micro-quiz HTML

1. Quelle partie contient le contenu visible principal : `head` ou `body` ?
2. Quelle balise représente un paragraphe ?
3. Quelle balise crée un lien ?
4. À quoi sert `href` ?
5. À quoi sert `src` sur une image ?
6. Pourquoi renseigner `alt` ?
7. Différence entre `ul` et `ol` ?
8. Dans quel dossier se trouve `photo.jpg` si `src="images/photo.jpg"` ?

---

# Jeudi — Réactivation

Faire afficher volontairement plusieurs extraits comportant une seule erreur chacun.

Exemples :

```html
<a href="formation.html>Formation</a>
```

```html
<img src="image/photo.jpg" alt="Photo">
```

alors que le dossier s'appelle `images`.

```html
<p>Bonjour<p>
```

Demander d'abord : « Qu'est-ce qui vous semble suspect ? » avant de donner la réponse.

---

# Gestion des étudiants rapides

Lorsqu'un étudiant termine :

1. il effectue la checklist de son propre travail ;
2. il réalise le challenge facultatif ;
3. il peut aider un camarade à condition de ne pas prendre son clavier ;
4. il peut améliorer la qualité de ses textes et de ses noms de fichiers.

Éviter de lui enseigner en avance CSS/JS au milieu de cette séance si cela crée un deuxième cours parallèle impossible à superviser.

---

# Jeudi — Bilan facultatif de fin de semaine

Si le rythme de la classe le permet, terminer par quelques questions identiques au diagnostic du lundi. La comparaison est plus intéressante qu'un score isolé.

Questions complémentaires possibles :

1. Que contient généralement `body` ?
2. Comment relier `index.html` à `contact.html` dans le même dossier ?
3. Si une image se trouve dans `images/photo.jpg`, quel chemin simple utiliser depuis `index.html` situé à la racine ?
4. Pourquoi tester réellement tous les liens ?
5. Pourquoi une page HTML simple peut-elle fonctionner sans CSS ?

Terminer par un bilan non noté : ce que chacun sait refaire seul / avec modèle / pas encore.
