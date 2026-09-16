# Présentation 4 — IP, DNS, URL, client-serveur et HTTP

**Durée cible : environ 70 minutes**  
**Nombre de slides : 28**

---

## Slide 1 — Comment retrouver un serveur sur Internet ?

Lorsque nous écrivons `www.wikipedia.org`, nous utilisons un nom facilement mémorisable. Pourtant, les réseaux informatiques doivent disposer d'informations d'adressage beaucoup plus précises pour acheminer les données.

Cette présentation ouvre la boîte noire entre le navigateur et le serveur. Nous allons découvrir cinq notions qui fonctionnent ensemble : **adresse IP, nom de domaine, DNS, URL et HTTP**.

Le but n'est pas de devenir administrateur réseau en une heure. Il s'agit d'acquérir un modèle mental suffisamment juste pour comprendre ce qui se passe lorsqu'un site fonctionne… ou ne fonctionne pas.

---

## Slide 2 — Une adresse permet d'identifier une destination réseau

Pour envoyer une lettre, il faut une adresse. Pour communiquer sur un réseau IP, les machines utilisent des **adresses IP**.

Une adresse IP participe à l'identification d'une interface sur un réseau et permet aux équipements réseau d'acheminer les paquets vers leur destination.

Pour commencer, nous utiliserons surtout l'image d'une « adresse réseau ». Elle n'est pas parfaite, mais elle permet de comprendre pourquoi le navigateur a besoin de davantage qu'un simple nom humain pour joindre un serveur.

**Visuel suggéré :** comparaison entre adresse postale et adresse IP, avec avertissement « analogie simplifiée ».

---

## Slide 3 — IPv4 : quatre nombres que vous avez peut-être déjà vus

Une adresse IPv4 est généralement écrite sous forme de quatre nombres séparés par des points, par exemple `192.168.1.25`.

Chaque nombre représente un octet, donc une valeur comprise entre 0 et 255. Une adresse IPv4 contient au total 32 bits.

À ce stade, nous n'étudierons ni les masques de sous-réseau ni le calcul binaire. Il suffit de reconnaître la forme générale d'une adresse IPv4 et de comprendre qu'elle joue un rôle dans l'adressage des communications.

**Exemple :** votre ordinateur possède très probablement une adresse IP sur le réseau de l'établissement.

---

## Slide 4 — Toutes les adresses IP ne sont pas visibles sur Internet

Sur un réseau local, on rencontre fréquemment des adresses dites **privées**, par exemple dans les plages `192.168.x.x` ou `10.x.x.x`.

Ces adresses sont utilisées à l'intérieur de réseaux privés et ne sont pas routées directement sur l'Internet public.

Une box ou un routeur peut permettre à plusieurs équipements privés de partager un accès vers Internet grâce à différents mécanismes que nous étudierons plus tard.

Pour cette semaine, retenez surtout qu'une adresse observée sur votre ordinateur n'est pas forcément une adresse directement joignable depuis le monde entier.

---

## Slide 5 — IPv6 : pourquoi avoir inventé d'autres adresses ?

IPv4 permet environ 4,3 milliards de valeurs d'adresses possibles. Cela semblait gigantesque au début d'Internet, mais le nombre d'équipements connectés a explosé.

IPv6 utilise des adresses beaucoup plus longues, sur 128 bits. Elles ressemblent par exemple à `2001:db8::1`.

Nous n'allons pas apprendre leur syntaxe cette semaine. Il est simplement important de savoir qu'Internet ne repose pas uniquement sur IPv4 et que l'évolution du réseau a nécessité un espace d'adressage beaucoup plus vaste.

**Visuel suggéré :** une petite boîte IPv4 face à une boîte IPv6 immense.

---

## Slide 6 — Les humains préfèrent les noms

Imaginez devoir retenir une adresse numérique différente pour chaque site que vous consultez. Ce serait extrêmement peu pratique.

Nous utilisons donc des **noms de domaine** comme `wikipedia.org`, `openstreetmap.org` ou `service-public.fr`.

Le nom est destiné à être plus stable et plus mémorisable pour les humains. Les informations techniques associées au service peuvent évoluer sans obliger tous les utilisateurs à apprendre une nouvelle adresse.

Cette séparation entre le nom logique d'un service et son implantation technique est extrêmement utile.

---

## Slide 7 — Un nom de domaine possède une structure hiérarchique

Prenons `www.exemple.fr`. On peut lire sa structure de droite à gauche.

`.fr` correspond à un domaine de premier niveau. `exemple` est le domaine enregistré sous `.fr`. `www` est ici un sous-domaine ou un nom d'hôte utilisé par l'organisation.

Cette organisation hiérarchique permet de répartir la gestion des noms. Il n'existe pas un immense fichier dans lequel une seule personne saisirait manuellement tous les noms d'Internet.

**Visuel suggéré :** arbre montrant racine → `.fr` → `exemple.fr` → `www.exemple.fr`.

---

## Slide 8 — Le DNS : un système distribué de noms

Le **Domain Name System**, DNS, fournit un système hiérarchique et distribué permettant d'associer des noms à différentes informations utiles.

Dans le cas le plus simple étudié ici, le navigateur a besoin de savoir comment joindre le serveur correspondant à un nom. Le DNS peut lui fournir les enregistrements nécessaires, notamment des adresses IP.

On compare souvent le DNS à un annuaire. L'image est pratique, mais retenez qu'il s'agit en réalité d'un système distribué, hiérarchique et beaucoup plus riche qu'un simple carnet d'adresses.

---

## Slide 9 — Pourquoi le DNS a-t-il été nécessaire ?

Aux débuts des réseaux Internet, une liste de noms de machines pouvait encore être maintenue dans un fichier partagé. À mesure que le nombre de machines augmentait, cette approche devenait difficile à maintenir et à distribuer.

Le DNS, décrit initialement par Paul Mockapetris en 1983, répond à ce problème de croissance en répartissant la responsabilité des différentes parties de l'espace de noms.

**Anecdote historique :** le DNS est donc né d'un problème que vous rencontrerez souvent en informatique : une solution simple fonctionne très bien… jusqu'au jour où l'échelle devient trop grande.

---

## Slide 10 — Résolution DNS : une version volontairement simplifiée

Lorsque vous demandez `www.exemple.fr`, votre machine s'appuie généralement sur un **résolveur DNS**. Celui-ci cherche ou obtient les informations nécessaires pour répondre à la question.

Selon la situation, la réponse peut déjà être présente dans un cache. Sinon, plusieurs serveurs DNS peuvent être interrogés jusqu'à obtenir les informations faisant autorité.

Pour cette semaine, retenez la chaîne mentale suivante : **nom demandé → résolution DNS → information permettant de joindre le service**.

Nous étudierons plus tard les serveurs racine, les zones, les caches et les types d'enregistrements.

---

## Slide 11 — Le cache évite de tout redemander constamment

Si chaque consultation d'un site obligeait à refaire toutes les étapes DNS depuis le début, cela générerait énormément de trafic inutile.

Les informations DNS peuvent donc être conservées temporairement dans différents caches. Tant qu'elles sont considérées comme valides, elles peuvent être réutilisées.

Cette optimisation explique aussi certains comportements déroutants : après une modification DNS, deux utilisateurs peuvent momentanément obtenir des réponses différentes selon les informations encore présentes dans leurs caches.

**Exemple :** un changement de serveur n'est pas toujours visible instantanément partout.

---

## Slide 12 — DNS en panne ne signifie pas forcément Internet en panne

Supposons que votre machine puisse communiquer avec une adresse IP distante mais qu'aucun nom de domaine ne soit résolu. La connexion réseau peut fonctionner alors que le service DNS utilisé rencontre un problème.

Pour l'utilisateur, le résultat ressemble pourtant à « Internet ne marche plus », car presque tous les services habituels sont appelés par leur nom.

Cette situation montre pourquoi un technicien cherche à distinguer les couches du problème au lieu d'utiliser une conclusion générale.

**Question à la classe :** si les noms ne fonctionnent plus mais que certaines adresses IP répondent, quel service peut-on suspecter ?

---

## Slide 13 — Une URL n'est pas seulement un nom de domaine

Une **URL** permet d'identifier une ressource et indique comment y accéder.

Prenons : `https://www.exemple.fr/cours/index.html`.

Cette adresse contient plusieurs informations : le schéma `https`, le nom d'hôte `www.exemple.fr` et le chemin `/cours/index.html`.

Le nom de domaine indique globalement vers quel service se tourner. Le chemin précise ensuite la ressource ou la route demandée sur ce service.

**Visuel suggéré :** URL découpée en blocs de couleurs avec légendes.

---

## Slide 14 — Le schéma : comment souhaite-t-on accéder à la ressource ?

Dans une URL Web, `http://` ou `https://` indique le schéma utilisé pour la communication.

Aujourd'hui, le Web public utilise très largement HTTPS, qui ajoute une protection cryptographique à la communication HTTP grâce à TLS.

Le schéma fait donc partie de l'adresse. Oublier ou modifier certaines parties d'une URL peut changer la manière dont le navigateur tente d'accéder à la ressource.

Pour cette semaine, retenez simplement : **HTTPS correspond à HTTP utilisé au sein d'une communication protégée par TLS**.

---

## Slide 15 — Le chemin désigne une ressource ou une route

Dans `https://exemple.fr/images/logo.png`, la partie `/images/logo.png` est le chemin demandé.

Sur un site très simple, ce chemin peut correspondre presque directement à un fichier stocké sur le serveur. Dans une application moderne, il peut aussi représenter une route logique traitée par un programme.

Cette distinction deviendra importante plus tard. Pour vos premiers sites HTML locaux, vous travaillerez essentiellement avec de vrais fichiers et de vrais dossiers : les chemins seront donc particulièrement concrets.

---

## Slide 16 — URL complète : d'autres éléments peuvent apparaître

Une URL peut également contenir un numéro de port, des paramètres de requête ou un fragment.

Exemple : `https://exemple.fr/recherche?q=html#resultats`.

Ici, `?q=html` contient un paramètre et `#resultats` désigne un fragment à l'intérieur de la ressource.

Nous n'utiliserons pas toutes ces possibilités cette semaine. L'objectif est simplement de ne plus considérer une URL comme une chaîne mystérieuse : elle possède une structure et chaque partie a un rôle.

---

## Slide 17 — Client et serveur : deux rôles, pas forcément deux types de machines

Dans le Web, le **client** initie généralement une demande. Le **serveur** fournit un service et répond aux demandes reçues.

Votre navigateur joue le rôle de client HTTP. Le serveur hébergeant le site joue le rôle de serveur HTTP.

Ces mots décrivent surtout des rôles. Une même machine peut être cliente dans une communication et serveur dans une autre.

Cette nuance évite un piège courant : imaginer qu'un « serveur » est obligatoirement une énorme machine spéciale enfermée dans un centre de données.

---

## Slide 18 — HTTP : le protocole de conversation du Web

**HTTP**, Hypertext Transfer Protocol, définit les règles utilisées pour les échanges entre clients et serveurs Web.

Un navigateur envoie une **requête HTTP**. Le serveur renvoie une **réponse HTTP**.

Le protocole définit notamment la méthode utilisée, la ressource demandée, des en-têtes décrivant le message et un éventuel contenu.

Pour un débutant, la notion essentielle est très simple : HTTP donne une structure commune aux demandes et aux réponses du Web.

**Visuel suggéré :** navigateur → « requête HTTP » → serveur → « réponse HTTP » → navigateur.

---

## Slide 19 — GET : demander une ressource

La méthode HTTP la plus intuitive est `GET`. Elle sert à demander la représentation d'une ressource.

Un navigateur pourrait, de manière très simplifiée, envoyer quelque chose comme :

```text
GET /index.html
```

Cela signifie : « Je souhaite obtenir la ressource `/index.html`. »

Une véritable requête HTTP contient davantage d'informations, mais cette ligne suffit à comprendre le principe.

Plus tard, vous découvrirez d'autres méthodes comme POST, PUT ou DELETE. Pour cette première semaine, GET permet déjà de comprendre le modèle.

---

## Slide 20 — La réponse contient un statut

Le serveur ne renvoie pas seulement du contenu. Il indique également comment la requête s'est passée grâce à un **code de statut HTTP**.

Ces codes sont regroupés en familles. Les `2xx` indiquent généralement un succès, les `3xx` une redirection, les `4xx` un problème lié à la requête ou à la ressource demandée, et les `5xx` une erreur côté serveur.

Vous n'avez pas à mémoriser des dizaines de codes. Nous allons simplement apprendre quelques classiques que vous rencontrerez souvent.

---

## Slide 21 — 200 : la requête a réussi

`200 OK` est l'un des statuts les plus courants. Il indique que la requête a été traitée avec succès et que la réponse contient généralement le résultat attendu.

Quand une page se charge normalement, vous ne voyez pas forcément ce code dans l'interface. Pourtant, le navigateur le reçoit dans les échanges HTTP.

Plus tard, les outils de développement du navigateur vous permettront d'observer directement ces requêtes et leurs statuts.

**Visuel suggéré :** carte verte « 200 OK — tout va bien ».

---

## Slide 22 — 404 : la ressource n'a pas été trouvée

`404 Not Found` signifie que le serveur a été joint, mais qu'il n'a pas trouvé la ressource demandée.

C'est une nuance très importante : une erreur 404 prouve généralement que la communication avec le serveur a déjà fonctionné jusqu'à un certain point.

Si vous demandez `/photo.jpg` alors que le fichier s'appelle réellement `photos.jpg`, le serveur peut parfaitement répondre… qu'il ne trouve pas ce que vous demandez.

**Anecdote à désamorcer :** l'histoire populaire selon laquelle « 404 » viendrait d'une salle 404 au CERN est un mythe. Le nombre appartient simplement à la classification des statuts HTTP.

---

## Slide 23 — 500 : cette fois, le serveur rencontre un problème

`500 Internal Server Error` indique que le serveur a rencontré une situation inattendue l'empêchant de traiter correctement la requête.

Contrairement au 404, le problème n'est pas simplement « la ressource demandée n'existe pas ». Une application ou un composant serveur a rencontré une erreur interne.

Pour l'utilisateur, les deux situations peuvent produire une page d'erreur. Pour le technicien, elles orientent le diagnostic dans des directions très différentes.

**Visuel suggéré :** comparaison 404 « ressource introuvable » / 500 « erreur côté serveur ».

---

## Slide 24 — HTTPS : protéger la communication

HTTP seul ne fournit pas le niveau de protection attendu aujourd'hui pour les communications sur le Web public. HTTPS combine HTTP avec TLS afin de protéger la communication entre client et serveur.

Cela permet notamment de chiffrer les données échangées et d'authentifier le serveur à l'aide de certificats.

Mais attention : **HTTPS ne signifie pas que le site est honnête ou sans danger**. Un site malveillant peut lui aussi disposer d'un certificat valide. HTTPS protège la communication ; il ne juge pas les intentions du propriétaire du site.

---

## Slide 25 — Un exemple complet : demander une page

Prenons `https://www.exemple.fr/cours.html`.

Le navigateur identifie le nom `www.exemple.fr`. Le système DNS aide à obtenir les informations permettant de joindre le service. Les paquets sont acheminés à travers les réseaux. Une communication protégée est établie pour HTTPS. Le navigateur envoie ensuite une requête HTTP pour `/cours.html`.

Le serveur traite cette requête et renvoie une réponse, par exemple avec le statut `200 OK` et un document HTML. Le navigateur interprète enfin ce document pour construire l'affichage.

**Visuel suggéré :** diagramme numéroté en six étapes.

---

## Slide 26 — Et si l'image de la page ne s'affiche pas ?

Le document HTML peut contenir une référence vers `images/chat.jpg`. Le navigateur effectue alors une nouvelle requête pour obtenir cette image.

Si le fichier n'existe pas à l'emplacement indiqué, la page HTML peut être chargée correctement tandis que la requête de l'image renvoie un `404`.

Cette situation sera très concrète dès mardi : lorsque vos images ne s'afficheront pas, le problème viendra souvent d'un nom de fichier ou d'un chemin incorrect, pas d'« Internet ».

---

## Slide 27 — Penser en chaîne aide à diagnostiquer

Lorsqu'un site ne fonctionne pas, un technicien cherche à savoir où la chaîne se brise.

L'ordinateur est-il connecté au réseau ? L'accès Internet fonctionne-t-il ? Le nom est-il résolu ? Le serveur répond-il ? Le statut HTTP indique-t-il une erreur ? La ressource demandée existe-t-elle ?

Cette méthode évite les diagnostics vagues. On remplace progressivement « ça ne marche pas » par une description précise du symptôme et de l'étape qui pose problème.

**Visuel suggéré :** chaîne avec cases à cocher réseau → DNS → serveur → HTTP → ressource.

---

## Slide 28 — Le modèle mental à retenir

Pour cette première semaine, retenez le scénario suivant :

**Une URL indique ce que je veux consulter. Le nom de domaine m'évite de mémoriser une adresse technique. Le DNS aide à retrouver les informations permettant de joindre le service. IP permet l'acheminement des communications entre réseaux. HTTP structure la requête et la réponse. Le navigateur interprète finalement la ressource reçue.**

Ce modèle est volontairement simplifié, mais il vous permettra déjà de comprendre beaucoup de situations réelles. Nous allons maintenant passer de la circulation des ressources à leur construction : de quoi une page Web est-elle faite ?
