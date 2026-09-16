# Cours — Informatique, Internet et Web

## 1. Qu'est-ce que l'informatique ?

Le mot informatique vient historiquement de l'idée de **traitement automatique de l'information**.

Prenons un exemple simple : une liste de températures `18`, `21`, `19`, `23` constitue des données. Si un programme calcule leur moyenne et indique « température moyenne : 20,25 °C », il transforme ces données pour produire une information utile.

On peut représenter très simplement :

```text
DONNEES -> TRAITEMENT -> INFORMATION
```

Dans une organisation, l'informatique ne se limite donc pas à écrire du code. Il faut également stocker, transporter, protéger, exploiter et mettre à disposition des informations.

---

## 2. Qu'est-ce qu'un système d'information ?

Une organisation — entreprise, association, école, hôpital, club sportif — utilise des informations pour fonctionner.

Son système d'information comprend les informations, les personnes, les procédures et les moyens techniques permettant de les utiliser.

Le système informatique est la partie technique qui participe à ce fonctionnement : ordinateurs, logiciels, réseaux, serveurs, bases de données, services en ligne, etc.

---

## 3. Qu'est-ce qu'un réseau ?

Un réseau informatique permet à plusieurs équipements de communiquer.

Chez vous, plusieurs appareils peuvent être connectés à la même box :

```text
Ordinateur -----\
Telephone ------- BOX / ROUTEUR ----- Internet
Console --------/
```

Ils forment un réseau local et peuvent accéder à d'autres réseaux grâce au routeur.

---

## 4. Qu'est-ce qu'Internet ?

Internet peut être présenté, à notre niveau, comme un **réseau mondial de réseaux interconnectés**.

Il ne s'agit donc pas d'un lieu unique ni d'un gigantesque ordinateur central.

Des millions d'équipements et de réseaux communiquent en suivant des protocoles communs.

Internet permet d'utiliser de nombreux services :

- le Web ;
- le courrier électronique ;
- la messagerie ;
- la visioconférence ;
- les jeux en ligne ;
- le transfert de fichiers ;
- de nombreux services professionnels.

---

## 5. Internet n'est pas le Web

C'est l'une des distinctions les plus importantes de cette semaine.

**Internet** est l'infrastructure de communication mondiale.

**Le Web** est un service qui utilise Internet pour permettre notamment la consultation de ressources reliées entre elles et accessibles avec un navigateur.

Une analogie imparfaite mais utile :

> Internet ressemble au réseau routier.
>
> Le Web ressemble à un type de transport qui utilise ces routes.

L'analogie a ses limites, mais elle aide à retenir que le Web utilise Internet sans être Internet tout entier.

---

## 6. Le navigateur

Un navigateur est un logiciel qui permet notamment de demander, recevoir et afficher des ressources Web.

Exemples : Firefox, Chrome, Edge, Safari.

Attention : **Google n'est pas un navigateur**. Google exploite notamment un moteur de recherche. Chrome est un navigateur développé par Google.

---

## 7. Client et serveur

Dans un échange Web simplifié :

- votre navigateur joue le rôle de **client** ;
- une machine ou un ensemble de machines distantes fournit le service : le **serveur**.

Le client demande une ressource. Le serveur traite la demande et répond.

```text
CLIENT  ---- requete ---->  SERVEUR
CLIENT  <--- reponse -----  SERVEUR
```

---

## 8. Adresse IP

Pour communiquer sur un réseau utilisant IP, les machines utilisent des adresses IP.

Pour cette première semaine, retenez simplement :

> une adresse IP permet d'identifier une interface réseau afin d'acheminer des communications.

Nous étudierons beaucoup plus précisément l'adressage et les réseaux plus tard.

---

## 9. Nom de domaine et DNS

Les humains mémorisent plus facilement des noms que des suites de nombres.

Un nom comme :

```text
www.wikipedia.org
```

est plus pratique à utiliser.

Le **DNS** permet notamment de résoudre un nom de domaine vers les informations nécessaires pour joindre le service, dont une adresse IP.

Image mentale utile : le DNS joue partiellement le rôle d'un annuaire.

---

## 10. URL

Une URL permet de désigner une ressource.

Exemple fictif :

```text
https://www.exemple.fr/cours/html/index.html
```

On peut y reconnaître :

- `https` : le schéma/protocole utilisé pour accéder à la ressource ;
- `www.exemple.fr` : le nom d'hôte ;
- `/cours/html/index.html` : le chemin vers la ressource.

Nous apprendrons plus tard des URL plus complexes avec paramètres et fragments.

---

## 11. HTTP

HTTP est un protocole utilisé pour les échanges du Web.

Le client envoie une **requête** ; le serveur fournit une **réponse**.

À notre niveau, imaginons :

```text
Je demande /index.html
```

et le serveur peut répondre :

```text
200 OK
```

Quelques codes célèbres :

- `200` : la requête a abouti ;
- `404` : la ressource demandée n'a pas été trouvée ;
- `500` : une erreur s'est produite côté serveur.

Il existe de nombreux autres codes. Vous n'avez pas à les apprendre aujourd'hui.

---

## 12. Que se passe-t-il quand je saisis une adresse ?

Modèle volontairement simplifié :

1. vous saisissez une URL ;
2. le navigateur doit déterminer où joindre le service ;
3. le DNS participe à la résolution du nom ;
4. des communications réseau sont établies ;
5. le navigateur envoie une requête ;
6. le serveur traite cette requête ;
7. il renvoie une réponse ;
8. le navigateur interprète les ressources reçues et affiche la page.

La réalité est plus complexe. Le but de cette première semaine est d'abord d'acquérir un modèle mental correct avant d'étudier progressivement les détails.