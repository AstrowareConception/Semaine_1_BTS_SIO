# Sources et vérification des anecdotes — Scripts de slides

Ce document accompagne les scripts de présentations. Il n'est pas destiné à être importé tel quel dans Gamma : il sert à conserver la provenance des principales informations historiques et techniques utilisées dans les anecdotes.

## Internet, ARPANET et TCP/IP

### Internet Society — A Brief History of the Internet

Source institutionnelle retraçant la naissance des concepts d'Internet, les travaux autour de TCP/IP, les premières applications et la transition d'ARPANET vers TCP/IP.

https://www.internetsociety.org/internet/history-internet/brief-history-internet/

Points utilisés dans les scripts :

- développement de l'architecture ouverte d'Internet ;
- rôle de TCP/IP ;
- importance historique du courrier électronique ;
- transition d'ARPANET de NCP à TCP/IP le 1er janvier 1983 ;
- anecdote des badges « I survived the TCP/IP transition ».

### UCLA — Leonard Kleinrock, The Day the Infant Internet Uttered its First Words

https://www.lk.cs.ucla.edu/internet_first_words.html

Point utilisé :

- le 29 octobre 1969 à 22 h 30, la tentative d'envoi de `LOGIN` entre UCLA et SRI s'interrompt après les caractères `L` et `O` lorsque le système plante ; le mot complet est transmis plus tard.

Cette source permet d'éviter de transformer l'anecdote « LO » en légende approximative.

---

## DNS

### IETF — RFC 882, Domain Names: Concepts and Facilities

https://datatracker.ietf.org/doc/html/rfc882

Paul Mockapetris, novembre 1983.

Points utilisés :

- introduction d'un espace de noms hiérarchique ;
- rôle des serveurs de noms ;
- besoin de disposer d'un système cohérent et distribué à mesure que l'Internet grandit.

Le RFC 882 est historique et a depuis été remplacé par des spécifications ultérieures. Il est utilisé ici uniquement pour expliquer la genèse du DNS.

---

## Naissance du World Wide Web

### CERN — The Birth of the Web

https://home.cern/science/computing/birth-web

### CERN — A Short History of the Web

https://home.cern/science/computing/the-birth-of-the-web/short-history-web

Points utilisés :

- Tim Berners-Lee invente le World Wide Web au CERN en 1989 ;
- première proposition en mars 1989 ;
- formalisation avec Robert Cailliau en 1990 ;
- premier serveur et premier navigateur opérationnels à la fin de 1990 ;
- le premier site est hébergé sur `info.cern.ch` ;
- le serveur NeXT porte une étiquette manuscrite demandant de ne pas l'éteindre ;
- le navigateur WorldWideWeb est également un éditeur ;
- mise du logiciel du Web dans le domaine public par le CERN le 30 avril 1993.

### W3C — A Little History of the World Wide Web

https://www.w3.org/History.html

Compléments chronologiques sur les années 1990-1991 et la diffusion des premiers navigateurs et serveurs Web.

---

## CSS

### W3C — A brief history of CSS until 2016

https://www.w3.org/Style/CSS20/history.html

Point utilisé :

- Håkon Wium Lie propose le concept des Cascading Style Sheets en 1994 alors qu'il travaille au CERN.

Cette anecdote est uniquement utilisée pour situer la séparation entre structure HTML et présentation CSS.

---

## HTML — bases techniques

### MDN Web Docs — HTML : Créer le contenu

https://developer.mozilla.org/fr/docs/Learn_web_development/Getting_started/Your_first_website/Creating_the_content

### MDN Web Docs — Syntaxe de base du HTML

https://developer.mozilla.org/fr/docs/Learn_web_development/Core/Structuring_content/Basic_HTML_syntax

### MDN Web Docs — HTML : HyperText Markup Language

https://developer.mozilla.org/fr/docs/Web/HTML

Points utilisés :

- rôle de HTML dans la structure du contenu ;
- notions d'élément, balise ouvrante, contenu, balise fermante et attribut ;
- rôles de `html`, `head`, `meta`, `title` et `body` ;
- utilisation de UTF-8 ;
- titres, paragraphes, listes, liens et images ;
- rôle de `href`, `src` et `alt` ;
- importance de la structure sémantique.

### WHATWG — HTML Living Standard

https://html.spec.whatwg.org/

Référence normative contemporaine du langage HTML. Elle est volontairement beaucoup trop détaillée pour les étudiants de cette première semaine, mais elle sert de garde-fou technique lors de la préparation du cours.

---

## Note sur les anecdotes et légendes urbaines

Les scripts évitent volontairement certaines histoires populaires lorsque leur origine est douteuse.

En particulier, **le code HTTP 404 ne vient pas d'une prétendue « salle 404 » du CERN**. Cette histoire circule depuis longtemps mais ne constitue pas une explication historique fiable. Dans le cours, `404` est présenté correctement comme un code de statut de la famille `4xx`.

De manière générale, les anecdotes utilisées dans les slides doivent servir la compréhension d'une notion et non remplacer l'explication technique.
