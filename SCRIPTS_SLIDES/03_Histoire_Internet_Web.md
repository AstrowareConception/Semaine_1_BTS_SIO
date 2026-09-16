# Présentation 3 — Une petite histoire d'Internet et du Web

**Durée cible : environ 45 minutes**  
**Nombre de slides : 18**

---

## Slide 1 — Internet n'est pas apparu d'un seul coup

Internet n'a pas été inventé un matin par une seule personne. Il résulte de plusieurs décennies de recherche sur les réseaux, les protocoles et le partage de ressources informatiques.

Le Web, lui, arrive beaucoup plus tard. Cette chronologie est essentielle : lorsqu'on confond Internet et le Web, on efface presque vingt ans d'histoire technique.

L'objectif de cette présentation n'est pas de retenir toutes les dates. Il est de comprendre comment une succession de problèmes concrets a conduit aux technologies que nous utilisons aujourd'hui.

**Visuel suggéré :** grande frise 1960 → 2026 avec quelques jalons seulement.

---

## Slide 2 — Années 1960 : les ordinateurs sont rares et coûteux

Dans les années 1960, les ordinateurs n'ont rien à voir avec nos machines personnelles. Ils sont immenses, coûteux et principalement utilisés par des universités, des administrations ou de grandes organisations.

Partager les ressources devient donc un enjeu majeur. Si plusieurs chercheurs éloignés géographiquement peuvent accéder aux mêmes machines ou échanger des informations, l'investissement devient beaucoup plus utile.

Cette époque voit se développer des recherches sur la manière de transmettre efficacement des données entre ordinateurs.

**Anecdote :** à cette époque, « utiliser un ordinateur » signifie souvent réserver du temps sur une machine partagée, pas ouvrir un ordinateur portable personnel.

---

## Slide 3 — Une idée essentielle : découper les messages en paquets

Une communication numérique peut être découpée en petits blocs appelés **paquets**. Chaque paquet peut être transmis à travers le réseau puis réassemblé à l'arrivée.

Cette approche est particulièrement adaptée aux réseaux informatiques : plusieurs communications peuvent partager les mêmes infrastructures et les données peuvent être acheminées de manière flexible.

Les recherches sur la commutation de paquets menées dans les années 1960 constituent l'une des briques fondamentales des réseaux modernes.

**Visuel suggéré :** un gros message découpé en cinq enveloppes numérotées puis réassemblé.

---

## Slide 4 — 1969 : ARPANET connecte ses premiers nœuds

ARPANET est l'un des réseaux pionniers à l'origine de l'histoire d'Internet. À l'automne 1969, plusieurs centres universitaires américains commencent à être reliés.

L'objectif n'est pas encore de créer le Web ni de permettre au grand public de regarder des vidéos. Il s'agit de faire communiquer des systèmes informatiques et de partager des ressources entre chercheurs.

ARPANET devient progressivement un terrain d'expérimentation pour de nouvelles formes de communication entre machines.

**Visuel suggéré :** carte très simplifiée des premiers nœuds américains d'ARPANET.

---

## Slide 5 — 29 octobre 1969 : le premier message s'arrête après « LO »

À UCLA, l'équipe de Leonard Kleinrock tente d'envoyer le mot `LOGIN` vers une machine du Stanford Research Institute. La lettre `L` arrive. Puis la lettre `O`. À la troisième lettre, le système distant plante.

Le premier message transmis lors de cette expérience n'est donc pas « LOGIN », mais simplement **« LO »**. Environ une heure plus tard, l'équipe parvient à envoyer le mot complet.

Cette anecdote est précieuse : même un moment historique de l'informatique commence par… un plantage.

**Anecdote à mettre fortement en valeur :** « Le premier message d'ARPANET n'a pas fonctionné du premier coup. »

---

## Slide 6 — Le courrier électronique devient rapidement essentiel

Les premiers réseaux sont pensés pour partager des ressources informatiques, mais les utilisateurs découvrent rapidement que communiquer entre humains est tout aussi utile.

Le courrier électronique devient l'une des applications les plus importantes des premiers réseaux. Il transforme la collaboration entre chercheurs et montre qu'un réseau informatique peut devenir un outil de communication sociale, pas seulement un moyen d'accéder à une machine distante.

Internet Society souligne que l'e-mail a probablement eu l'un des impacts les plus importants parmi les premières applications réseau.

---

## Slide 7 — Le problème : plusieurs réseaux différents doivent communiquer

Créer un réseau est une chose. Faire communiquer **des réseaux différents** en est une autre.

Dans les années 1970, différentes technologies réseau existent. Elles n'utilisent pas forcément les mêmes règles internes. Robert Kahn puis Vint Cerf travaillent sur une architecture permettant de relier ces réseaux sans imposer qu'ils deviennent tous identiques.

C'est une idée fondamentale d'Internet : chaque réseau peut conserver son fonctionnement interne tout en utilisant des protocoles communs pour communiquer avec les autres.

**Visuel suggéré :** trois réseaux de formes différentes reliés par des passerelles.

---

## Slide 8 — TCP/IP : une langue commune entre réseaux

Les travaux menés dans les années 1970 aboutissent progressivement à la suite de protocoles que nous appelons aujourd'hui **TCP/IP**.

IP s'occupe notamment de l'adressage et de l'acheminement des paquets entre réseaux. TCP fournit, pour les applications qui l'utilisent, des mécanismes permettant notamment d'obtenir une communication fiable et ordonnée.

Nous ne détaillerons pas ces protocoles cette semaine. L'idée importante est qu'une communication mondiale devient possible parce que des systèmes différents acceptent de parler des langages communs.

---

## Slide 9 — 1er janvier 1983 : une migration géante

Le 1er janvier 1983, les machines d'ARPANET doivent passer de l'ancien protocole NCP à TCP/IP. Cette transition est parfois considérée comme un jalon majeur dans l'histoire d'Internet.

Elle ressemble à une migration informatique moderne : il faut préparer les systèmes afin qu'ils adoptent les nouvelles règles au même moment.

**Anecdote réelle :** la transition avait été planifiée pendant plusieurs années et des badges « I survived the TCP/IP transition » ont même été distribués. Cela rappelle qu'une migration critique n'est jamais seulement une affaire de code : elle exige coordination et préparation.

---

## Slide 10 — 1983 : le DNS répond à un problème de croissance

Lorsque le nombre de machines augmente, maintenir manuellement une simple liste reliant tous les noms de machines à leurs adresses devient de moins en moins réaliste.

En 1983, Paul Mockapetris décrit dans les RFC 882 et 883 les concepts du **Domain Name System**, le DNS. Le système repose sur un espace de noms hiérarchique et distribué.

Cette invention permet au réseau de continuer à grandir sans dépendre d'un unique fichier de correspondances maintenu manuellement.

**Visuel suggéré :** arbre DNS très simplifié partant de la racine vers `.fr`, `.org`, puis des domaines.

---

## Slide 11 — Dans les années 1980, Internet existe déjà… sans Web

À la fin des années 1980, des réseaux interconnectés utilisent TCP/IP, le courrier électronique existe, le DNS existe et des utilisateurs transfèrent des fichiers ou se connectent à distance.

Pourtant, personne n'a encore ouvert Wikipédia, Google ou un site Web : le World Wide Web n'existe pas.

C'est le meilleur moyen de retenir la différence entre les deux notions : **Internet est plus ancien que le Web**.

**Question à poser :** si le Web disparaissait, pourrait-on encore imaginer d'autres services utilisant Internet ? Oui.

---

## Slide 12 — 1989 : un problème de scientifiques au CERN

Au CERN, des milliers de scientifiques provenant de nombreux pays collaborent. Les informations existent, mais elles sont dispersées dans différentes machines, documents et systèmes.

Tim Berners-Lee cherche une manière simple de relier ces informations. En mars 1989, il rédige une première proposition qui combine plusieurs idées existantes : réseaux, ordinateurs et hypertexte.

Son objectif initial n'est pas de créer les réseaux sociaux ou le commerce électronique. Il cherche d'abord à faciliter le partage d'informations entre chercheurs.

**Visuel suggéré :** documents scientifiques reliés entre eux par des liens.

---

## Slide 13 — Le Web repose sur trois briques simples mais puissantes

Le projet World Wide Web associe trois concepts fondamentaux :

**URL** permet d'identifier une ressource. **HTTP** définit une manière d'échanger des ressources entre client et serveur. **HTML** permet de structurer des documents contenant notamment des liens hypertextes.

Aucune de ces briques n'a besoin de connaître tout le Web. Ensemble, elles permettent pourtant de construire progressivement un système mondial de documents reliés.

Cette simplicité initiale est l'une des raisons pour lesquelles le Web a pu se diffuser largement.

---

## Slide 14 — 1990 : le premier navigateur est aussi un éditeur

À la fin de 1990, Tim Berners-Lee dispose au CERN d'un premier serveur Web et d'un navigateur appelé **WorldWideWeb**, développé sur une machine NeXT.

Ce navigateur n'est pas seulement conçu pour consulter des pages : il permet aussi d'en éditer. À l'origine, le Web est donc imaginé comme un espace où l'on peut à la fois lire et produire de l'information.

**Anecdote :** avant que « navigateur Web » ne devienne synonyme de consommation de contenu, l'un des tout premiers navigateurs était également un outil d'édition.

---

## Slide 15 — Le premier serveur portait une consigne très claire

Le premier serveur Web fonctionnait sur l'ordinateur NeXT de Tim Berners-Lee au CERN. Une étiquette manuscrite rouge avertissait : **« This machine is a server. DO NOT POWER IT DOWN!! »**

Cette phrase semble presque comique aujourd'hui, mais elle exprime une réalité toujours actuelle : un service dépend d'une infrastructure qui doit rester disponible.

Le premier site Web, hébergé sur `info.cern.ch`, expliquait d'ailleurs le projet World Wide Web lui-même.

**Visuel suggéré :** photographie ou illustration de la machine NeXT avec son étiquette.

---

## Slide 16 — 1993 : le Web devient beaucoup plus facile à diffuser

Le 30 avril 1993, le CERN place le logiciel du World Wide Web dans le domaine public puis propose une version sous licence ouverte. Cette décision contribue fortement à sa diffusion.

La même période voit apparaître des navigateurs comme Mosaic, qui rendent le Web plus agréable à utiliser et popularisent notamment l'intégration d'images dans les pages.

Le Web commence alors à sortir du monde académique pour toucher un public beaucoup plus large.

**Anecdote :** quelques années seulement séparent un outil destiné aux chercheurs d'une révolution mondiale de la communication.

---

## Slide 17 — Le Web devient une plateforme

Dans les années suivantes apparaissent moteurs de recherche, commerce électronique, médias en ligne, réseaux sociaux, applications Web, vidéo en streaming, services cloud et outils collaboratifs.

Le Web n'est plus seulement un ensemble de documents à lire. Il devient une plateforme sur laquelle on travaille, communique, achète, joue, apprend et développe des services complexes.

Les technologies évoluent énormément, mais les idées fondamentales restent reconnaissables : des ressources identifiées par des adresses, des clients, des serveurs, des protocoles et des liens.

---

## Slide 18 — Une histoire à retenir en cinq étapes

Pour cette première semaine, retenez cinq grands repères plutôt qu'une longue liste de dates.

**1969 :** ARPANET relie ses premiers nœuds et « LO » devient une anecdote célèbre.  
**Années 1970 :** émergence des idées menant à TCP/IP.  
**1983 :** transition d'ARPANET vers TCP/IP et naissance conceptuelle du DNS.  
**1989-1990 :** Tim Berners-Lee conçoit puis met en œuvre le World Wide Web au CERN.  
**1993 :** l'ouverture du Web et l'essor des navigateurs accélèrent sa diffusion.

La leçon principale est simple : **Internet est l'infrastructure historique ; le Web est une invention ultérieure construite dessus.**
