# Présentation 8 — Consolider son HTML et résoudre les erreurs fréquentes

**Durée cible : environ 30 minutes**  
**Nombre de slides : 12**

---

## Slide 1 — Quand « ça ne marche pas », on commence par décrire

En informatique, « ça ne marche pas » n'est pas un diagnostic. C'est seulement le point de départ.

Une description utile précise ce qui était attendu, ce qui se produit réellement et dans quel contexte.

Par exemple : « Quand je clique sur le lien Formation depuis `index.html`, le navigateur affiche une page introuvable » est beaucoup plus exploitable que « mon site est cassé ».

Cette habitude va vous faire gagner énormément de temps dès cette semaine.

---

## Slide 2 — Première question : ai-je enregistré le bon fichier ?

Avant de chercher une erreur compliquée, vérifiez les causes simples.

Avez-vous enregistré le fichier ? Travaillez-vous bien dans le fichier que le navigateur affiche ? Le dossier ouvert dans VS Code est-il celui que vous croyez ?

Beaucoup de débutants modifient une copie du fichier tandis que le navigateur en affiche une autre.

**Réflexe :** identifier précisément le chemin du fichier ouvert dans VS Code et celui affiché dans le navigateur.

---

## Slide 3 — Deuxième question : le nom du fichier est-il exact ?

Un lien vers :

```html
<a href="formation.html">Formation</a>
```

ne peut fonctionner que si la ressource demandée porte réellement ce nom à l'emplacement attendu.

Vérifiez les fautes de frappe, l'extension et les majuscules.

`formation.html`, `formations.html`, `Formation.html` et `formation.htm` ne sont pas forcément équivalents.

**Anecdote de terrain :** relire lentement le nom du fichier caractère par caractère résout parfois un problème qui semblait mystérieux depuis dix minutes.

---

## Slide 4 — Troisième question : le chemin part-il du bon endroit ?

Un chemin relatif doit être interprété depuis le fichier courant.

Si `formation.html` se trouve dans un sous-dossier `pages`, alors :

```html
<a href="pages/formation.html">Formation</a>
```

peut fonctionner depuis `index.html` situé à la racine.

Mais le même chemin copié dans une page déjà située dans `pages` ne désigne plus le même emplacement.

**Méthode :** dessinez l'arborescence sur papier si nécessaire. Ce n'est pas « tricher », c'est raisonner.

---

## Slide 5 — Une image cassée est souvent un problème de chemin

Si le navigateur affiche l'icône d'une image manquante, vérifiez d'abord :

- le fichier existe-t-il ?
- son nom est-il exactement celui indiqué dans `src` ?
- est-il dans le bon dossier ?
- le chemin est-il calculé depuis la bonne page ?

Ne modifiez pas dix choses à la fois. Testez une hypothèse, observez le résultat puis continuez.

Cette méthode évite de créer de nouvelles erreurs en essayant de corriger la première.

---

## Slide 6 — Vérifier les balises ouvrantes et fermantes

Un élément classique possède souvent une ouverture et une fermeture :

```html
<p>Mon paragraphe</p>
```

Une balise oubliée ou mal écrite peut perturber la structure du document.

Lorsque le résultat devient étrange, relisez les paires de balises et leur imbrication.

L'indentation aide énormément : si les niveaux sont visuellement cohérents, les éléments mal fermés deviennent plus faciles à repérer.

---

## Slide 7 — Vérifier les guillemets des attributs

Les attributs suivent généralement cette forme :

```html
nom="valeur"
```

Exemple :

```html
<a href="contact.html">Contact</a>
```

Un guillemet oublié peut conduire le navigateur à interpréter de travers la suite de la balise.

Lorsqu'un lien ou une image semble incorrect, relisez entièrement la balise au lieu de regarder uniquement la valeur du chemin.

**Visuel suggéré :** même balise correcte puis version avec guillemet manquant entouré en rouge.

---

## Slide 8 — Modifier une seule chose à la fois

Face à un problème, le réflexe débutant est parfois de modifier plusieurs lignes au hasard jusqu'à ce que « ça marche ».

Cette stratégie empêche de comprendre la cause réelle.

Préférez une démarche simple : **observer → proposer une hypothèse → modifier un élément → tester → conclure**.

Si le test ne change rien, vous avez appris quelque chose : l'hypothèse était probablement mauvaise. Vous pouvez alors revenir en arrière et en tester une autre.

C'est déjà une forme de méthode expérimentale appliquée au développement.

---

## Slide 9 — Les commentaires peuvent aider à organiser le fichier

HTML permet d'écrire des commentaires :

```html
<!-- Navigation principale -->
```

Le navigateur n'affiche pas ce texte comme contenu de la page. Le commentaire sert aux personnes qui lisent le code.

Dans un fichier débutant, quelques commentaires peuvent aider à repérer les grandes zones : navigation, présentation, centres d'intérêt, pied de page.

Il ne faut pas commenter chaque balise évidente. Le commentaire doit apporter une information utile à la lecture du document.

---

## Slide 10 — Tester comme un utilisateur

Une page n'est pas terminée parce que son auteur pense qu'elle fonctionne.

Ouvrez-la réellement. Cliquez sur tous les liens. Vérifiez toutes les images. Passez d'une page à l'autre. Essayez d'arriver directement sur une page secondaire puis de revenir vers l'accueil.

Cette vérification s'appelle déjà, à petite échelle, une forme de **recette** ou de test d'acceptation.

Jeudi, une autre équipe testera votre site. Elle trouvera peut-être des problèmes auxquels vous n'aviez pas pensé : c'est précisément l'intérêt du test croisé.

---

## Slide 11 — Savoir demander de l'aide fait partie de la compétence

Avant d'appeler l'enseignant, préparez trois informations :

1. ce que vous essayez de faire ;
2. ce que vous observez ;
3. ce que vous avez déjà vérifié.

Exemple : « Je veux afficher `logo.png`. Le texte alternatif apparaît mais pas l'image. J'ai vérifié que le fichier existe dans `images`, mais je ne suis pas sûr de mon chemin. »

Une demande précise permet d'être aidé plus vite et montre que vous avez déjà commencé à diagnostiquer.

---

## Slide 12 — Le vrai objectif : devenir progressivement autonome

Le but n'est pas de ne plus jamais rencontrer d'erreur. Même les professionnels rencontrent des erreurs tous les jours.

Le but est de devenir capable de transformer un problème vague en problème précis, puis de tester méthodiquement des solutions.

Pour cette semaine, votre checklist mentale peut rester très courte : **enregistrer → vérifier le fichier → vérifier le nom → vérifier le chemin → vérifier la syntaxe → tester**.

Si vous apprenez déjà ce réflexe en même temps que vos premières balises HTML, vous construisez une compétence bien plus importante que la mémorisation d'une dizaine de balises.
