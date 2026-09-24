# Scripts de présentations — Semaine 1 BTS SIO

Ce dossier contient les scripts destinés à être importés ou adaptés dans **Gamma** afin de produire les présentations projetées pendant la première semaine intensive.

Les documents sont volontairement rédigés **slide par slide**, avec un titre explicite et un contenu formulé sous forme de texte. L'objectif n'est pas de transformer chaque slide en mur de texte : Gamma pourra condenser, hiérarchiser et mettre en forme ces contenus. Le script constitue la matière pédagogique complète à préserver.

## Hypothèse de rythme

La semaine est construite sur l'hypothèse suivante : **une slide correspond en moyenne à 2 à 3 minutes de cours**. Une présentation de 20 slides représente donc environ 45 à 55 minutes de cours, en tenant compte des questions, exemples et petites interactions.

Les temps de démonstration, les quiz, les exercices et les phases de pratique ne sont pas comptés comme des slides de cours.

## Présentations prévues

| N° | Présentation | Slides | Durée cible |
|---:|---|---:|---:|
| 1 | [Découvrir l'informatique et le BTS SIO](01_Culture_informatique.md) | 16 | ~40 min |
| 2 | [Internet et le Web : comprendre ce qui se passe derrière l'écran](02_Internet_et_Web.md) | 24 | ~60 min |
| 3 | [Une petite histoire d'Internet et du Web](03_Histoire_Internet_Web.md) | 18 | ~45 min |
| 4 | [IP, DNS, URL, client-serveur et HTTP](04_IP_DNS_URL_HTTP.md) | 28 | ~70 min |
| 5 | [De quoi est faite une page Web ? Fichiers, dossiers et VS Code](05_Technologies_Web_Fichiers_VSCode.md) | 20 | ~50 min |
| 6 | [Les bases de HTML](06_Bases_HTML.md) | 28 | ~70 min |
| 7 | [Liens, images, chemins et site multi-pages](07_Liens_Images_Multipages.md) | 22 | ~55 min |
| 8 | [Consolider son HTML et résoudre les erreurs fréquentes](08_Consolidation_Debug_HTML.md) | 12 | ~30 min |

**Total : 168 slides, soit environ 7 heures de contenu projeté.**

Le reste des **24 heures** est volontairement réservé à la pratique. Pour ce public débutant, le cours projeté ne doit jamais absorber l'essentiel du temps disponible.

## Répartition conseillée sur les trois journées

- **Lundi** : présentations 1 à 4, entrecoupées de quiz, échanges et activités.
- **Mardi** : présentations 5, 6 et début de la 7, avec de nombreuses manipulations dans VS Code.
- **Jeudi** : fin éventuelle de la présentation 7 et présentation 8, puis laboratoire de pratique : 48 exercices, ateliers de débogage, parcours différenciés et mini-projet.

## Convention de rédaction pour Gamma

Chaque document suit la structure :

```markdown
## Slide 1 — Titre de la slide

Texte rédigé qui constitue la matière principale à faire apparaître sur la slide.

**Anecdote / exemple :** éventuel contenu à mettre en valeur dans un encadré.

**Visuel suggéré :** indication destinée à guider Gamma.

---
```

Les anecdotes sont intégrées lorsqu'elles ont un véritable intérêt pédagogique. Elles servent à donner de la chair aux notions : premier message d'ARPANET interrompu après deux lettres, premier serveur Web portant une étiquette demandant de ne surtout pas l'éteindre, transition TCP/IP du 1er janvier 1983, etc.

## Conseils d'utilisation dans Gamma

- Importer **une présentation à la fois** plutôt que l'ensemble du dossier.
- Demander à Gamma de conserver **une section par titre `Slide X`**.
- Préférer une mise en page très visuelle, avec peu de texte affiché simultanément, mais sans supprimer les idées du script.
- Demander des schémas simples lorsqu'ils sont suggérés : client/serveur, DNS, arborescence de fichiers, anatomie d'une balise HTML.
- Éviter les captures d'écran artificielles de logiciels : pour VS Code, une démonstration réelle en classe restera plus pertinente.
- Conserver les anecdotes sous forme d'encadrés ou de cartes « Le saviez-vous ? ».

## Sources historiques et techniques

Les anecdotes historiques ont été vérifiées principalement à partir de sources institutionnelles ou techniques : CERN, Internet Society, UCLA, IETF, W3C et MDN Web Docs. Un document de références est fourni dans [SOURCES.md](SOURCES.md).
