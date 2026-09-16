# Présentation 2 — Internet et le Web : comprendre ce qui se passe derrière l'écran

**Durée cible : environ 60 minutes**  
**Nombre de slides : 24**

---

## Slide 1 — Internet et le Web ne sont pas la même chose

Dans le langage courant, on emploie souvent « Internet » et « Web » comme des synonymes. Techniquement, ce sont pourtant deux notions différentes.

**Internet** est un immense réseau de réseaux permettant à des machines de communiquer. **Le Web** est l'un des services qui utilisent cette infrastructure pour permettre la consultation de ressources reliées entre elles par des liens.

Comprendre cette distinction est indispensable : Internet existait avant le Web et continuerait à transporter d'autres services même si aucun site Web n'existait.

**Visuel suggéré :** Internet représenté comme une autoroute, avec le Web comme l'un des types de véhicules qui l'utilisent.

---

## Slide 2 — Un réseau, avant Internet

Un réseau informatique est un ensemble d'équipements capables d'échanger des données. Deux ordinateurs reliés entre eux forment déjà un réseau très simple.

Dans une salle de cours, les ordinateurs peuvent être connectés à un même réseau local. Celui-ci peut comprendre des postes, des imprimantes, un point d'accès Wi-Fi, un commutateur et une box ou un routeur.

Le réseau permet de partager des ressources et de communiquer. Internet consiste ensuite à relier entre eux un très grand nombre de réseaux différents.

**Visuel suggéré :** petit réseau local avec trois PC, une imprimante, un switch et un routeur.

---

## Slide 3 — Pourquoi relier des réseaux entre eux ?

Un réseau local est utile, mais il reste limité aux équipements qui y sont directement ou indirectement connectés. Pour communiquer avec une machine située dans une autre école, une autre ville ou un autre pays, il faut pouvoir traverser plusieurs réseaux.

L'idée fondatrice d'Internet est précisément de permettre à des réseaux différents de communiquer ensemble selon des règles communes.

Le mot **Internet** vient d'ailleurs de l'idée d'« inter-networking » : faire communiquer des réseaux entre eux.

**Exemple :** votre ordinateur peut être connecté au Wi-Fi de l'établissement tout en accédant à un serveur situé dans un centre de données à plusieurs centaines de kilomètres.

---

## Slide 4 — Votre ordinateur n'est pas directement relié à tous les autres

Quand vous consultez un site situé aux États-Unis, aucun câble ne relie directement votre ordinateur personnel au serveur concerné. Les données traversent une succession d'équipements et de réseaux.

Le trajet peut être résumé ainsi : **ordinateur → réseau local → routeur → fournisseur d'accès → autres réseaux → réseau de destination → serveur**.

Chaque étape transmet les données vers l'étape suivante. Internet fonctionne donc davantage comme un réseau routier mondial composé d'innombrables routes interconnectées que comme un câble gigantesque reliant chaque machine à toutes les autres.

---

## Slide 5 — Le rôle de la box et du routeur

À la maison, la box Internet remplit plusieurs fonctions. Elle permet notamment à vos équipements de rejoindre un réseau local, puis d'accéder au réseau de votre fournisseur d'accès.

Le **routeur** est l'équipement chargé d'orienter les données entre différents réseaux. Il examine où les données doivent aller et les transmet vers une route appropriée.

Dans les infrastructures professionnelles et sur Internet, cette fonction est assurée par de nombreux routeurs spécialisés.

**Visuel suggéré :** maison avec téléphone, ordinateur et console reliés à une box, puis vers Internet.

---

## Slide 6 — Le fournisseur d'accès à Internet

Votre réseau local doit rejoindre Internet par l'intermédiaire d'un opérateur : le **fournisseur d'accès à Internet**, souvent abrégé FAI.

Le FAI connecte ses abonnés à son propre réseau, lui-même interconnecté à d'autres réseaux. Orange, Free, SFR ou Bouygues Telecom sont des exemples connus en France, mais de nombreux autres opérateurs existent.

Le fournisseur d'accès n'est donc pas « Internet ». Il constitue l'une des portes permettant d'y accéder.

**Question à la classe :** lorsqu'une box tombe en panne, est-ce Internet qui est en panne ? Non : c'est votre accès à Internet qui est interrompu.

---

## Slide 7 — Internet n'a pas un centre unique

Internet n'est pas une entreprise possédant un ordinateur central mondial. Il résulte de l'interconnexion de nombreux réseaux appartenant à des opérateurs, entreprises, universités, administrations et fournisseurs de services.

Il existe évidemment des organisations chargées de coordonner certaines ressources et des acteurs possédant des infrastructures extrêmement importantes. Mais le réseau lui-même est fondamentalement distribué.

Cette architecture explique une partie de sa robustesse : plusieurs chemins peuvent parfois permettre d'atteindre une même destination.

**Visuel suggéré :** carte de nombreux réseaux reliés entre eux, sans centre unique.

---

## Slide 8 — Internet transporte des données, pas seulement des pages Web

Lorsque l'on pense à Internet, on pense spontanément aux sites Web. Pourtant Internet transporte bien d'autres types de communications.

Le courrier électronique, certains jeux en ligne, les appels audio ou vidéo, le transfert de fichiers, la synchronisation d'un cloud, les mises à jour logicielles et de nombreux objets connectés utilisent Internet.

Le Web est donc **un service parmi d'autres** fonctionnant au-dessus de l'infrastructure Internet.

**Exemple :** lorsque votre client de messagerie récupère un e-mail, il utilise Internet, mais il n'est pas obligé d'utiliser le Web pour transporter ce courrier.

---

## Slide 9 — Alors, qu'est-ce que le Web ?

Le World Wide Web est un système permettant de consulter des ressources identifiées par des adresses et reliées entre elles par des liens hypertextes.

Une ressource Web peut être une page, une image, un fichier, une vidéo ou une donnée fournie par un service.

Pour consulter le Web, l'utilisateur emploie généralement un **navigateur**. Celui-ci demande des ressources à des **serveurs Web**, puis interprète les réponses reçues afin de les présenter à l'écran.

Le Web repose notamment sur trois idées historiques majeures : l'URL pour identifier les ressources, HTTP pour les échanges et HTML pour structurer les documents.

---

## Slide 10 — Pourquoi parle-t-on de « toile » ?

Le mot anglais **web** signifie « toile ». L'image vient du fait que les documents peuvent se relier entre eux grâce aux liens hypertextes.

Une page peut pointer vers dix autres pages ; chacune de ces pages peut en pointer vers d'autres. On obtient progressivement un réseau de documents reliés, semblable à une immense toile.

Le lien est donc l'une des inventions les plus importantes du Web. Il permet de passer d'une ressource à une autre sans connaître à l'avance l'organisation physique des serveurs.

**Visuel suggéré :** graphe de pages reliées par des liens, comme une toile.

---

## Slide 11 — Le navigateur : votre client Web

Chrome, Firefox, Edge ou Safari sont des **navigateurs Web**. Leur rôle ne consiste pas seulement à « afficher Internet ».

Le navigateur sait demander des ressources à des serveurs, recevoir leurs réponses, interpréter du HTML, appliquer du CSS, exécuter du JavaScript et construire l'affichage final.

Il assure également de nombreuses fonctions de sécurité, de stockage local, de gestion de certificats et de confidentialité.

Pour commencer, retenons surtout ceci : **le navigateur est le logiciel client qui vous permet d'utiliser le Web**.

---

## Slide 12 — Un moteur de recherche n'est pas un navigateur

Google est souvent confondu avec Chrome. Pourtant, Google Search est un **moteur de recherche**, alors que Chrome est un **navigateur**.

Le navigateur est le logiciel qui consulte des ressources Web. Le moteur de recherche est un service Web qui indexe de nombreuses pages et aide l'utilisateur à les retrouver.

On peut utiliser Google Search depuis Firefox, Edge ou Safari. Inversement, on peut utiliser Chrome sans passer par Google Search, simplement en saisissant directement l'adresse d'un site.

**Petit défi :** demander aux étudiants de citer deux navigateurs et deux moteurs de recherche différents.

---

## Slide 13 — Le serveur : la machine qui répond

Un serveur est un système qui fournit un service à d'autres machines appelées clients. Dans le cas du Web, un serveur Web reçoit des demandes et renvoie les ressources correspondantes.

Le mot « serveur » peut désigner la machine physique, une machine virtuelle ou le logiciel qui écoute les requêtes. À ce stade, il suffit de retenir l'idée de rôle : le client demande, le serveur répond.

Un même serveur physique peut héberger plusieurs services, et un grand site peut au contraire utiliser des milliers de machines.

**Visuel suggéré :** plusieurs navigateurs envoyant des demandes vers un serveur central.

---

## Slide 14 — Client et serveur : une conversation

Le fonctionnement du Web peut être résumé comme une conversation.

Le client dit en substance : « Je voudrais cette ressource. » Le serveur examine la demande puis répond : « Voici la ressource », « Je ne la trouve pas » ou « J'ai rencontré un problème ».

Cette logique de **requête / réponse** est fondamentale. Elle reviendra en développement Web, en administration réseau, dans les API et dans de nombreux autres domaines.

**Visuel suggéré :** deux personnages, « navigateur » et « serveur », échangeant une requête puis une réponse.

---

## Slide 15 — Quand vous tapez une adresse, plusieurs choses se passent

Saisir une adresse dans un navigateur semble instantané, mais plusieurs opérations s'enchaînent en quelques fractions de seconde.

Le navigateur doit comprendre l'adresse demandée, déterminer où se trouve le serveur, établir une communication, envoyer une requête, attendre une réponse, récupérer plusieurs ressources puis construire l'affichage.

Une page moderne peut déclencher des dizaines, parfois des centaines de requêtes pour récupérer HTML, images, feuilles de style, scripts, polices et données.

L'impression d'une seule « page » masque donc une activité réseau importante.

---

## Slide 16 — Étape 1 : l'utilisateur formule une demande

Tout commence par une action : saisir une URL, cliquer sur un lien ou utiliser un favori.

Par exemple : `https://www.wikipedia.org/`.

Le navigateur analyse cette adresse. Il identifie notamment le protocole demandé et le nom du serveur à contacter.

Pour l'utilisateur, c'est une simple chaîne de caractères. Pour le navigateur, cette adresse contient les informations nécessaires pour commencer à rechercher la ressource.

**Visuel suggéré :** barre d'adresse d'un navigateur avec différentes parties mises en évidence.

---

## Slide 17 — Étape 2 : retrouver la machine

Les humains préfèrent utiliser des noms comme `wikipedia.org`, alors que les communications réseau reposent notamment sur des adresses IP.

Le système DNS aide à faire le lien entre ces noms et les informations nécessaires pour joindre les serveurs concernés.

On peut comparer cette étape à la recherche d'un contact dans un carnet d'adresses : vous connaissez le nom de la personne, puis vous retrouvez son numéro.

Cette comparaison est imparfaite, mais elle permet de comprendre le principe général avant d'étudier le DNS plus précisément.

---

## Slide 18 — Étape 3 : traverser les réseaux

Une fois la destination connue, les données quittent votre réseau local. Elles peuvent traverser plusieurs routeurs et plusieurs réseaux avant d'arriver au serveur.

Le trajet n'est pas nécessairement identique à chaque instant. Les opérateurs utilisent des mécanismes de routage pour déterminer comment atteindre les différents réseaux d'Internet.

À notre niveau, il n'est pas nécessaire de connaître ces protocoles. Il faut simplement comprendre qu'une communication distante implique une succession de transmissions intermédiaires.

**Visuel suggéré :** chemin en plusieurs sauts entre un ordinateur et un serveur distant.

---

## Slide 19 — Étape 4 : le serveur reçoit la requête

Le serveur reçoit une demande provenant du navigateur. Dans le cas le plus simple, il recherche le fichier correspondant et le renvoie.

Dans une application moderne, la réponse peut être produite dynamiquement. Le serveur peut consulter une base de données, vérifier un compte utilisateur, effectuer un calcul puis générer une réponse spécifique.

Deux utilisateurs qui demandent la même URL peuvent ainsi recevoir des contenus différents selon leur compte ou leur situation.

Cette distinction entre contenu statique et contenu dynamique sera étudiée plus tard dans la formation.

---

## Slide 20 — Étape 5 : le navigateur reçoit des ressources

Le navigateur reçoit d'abord une réponse, souvent un document HTML. En lisant ce document, il découvre qu'il doit parfois demander d'autres ressources : images, CSS, JavaScript, polices ou données supplémentaires.

Il réalise alors de nouvelles requêtes.

Le navigateur assemble progressivement tous ces éléments pour construire la page visible à l'écran.

**Exemple :** une image déclarée dans le HTML n'est généralement pas « contenue » dans le fichier HTML. Le navigateur doit la télécharger séparément à partir de son adresse.

---

## Slide 21 — Une page Web n'est pas une capture d'écran

Une page Web n'est pas envoyée au navigateur comme une grande photographie déjà terminée.

Le serveur fournit principalement des ressources et des instructions de structure ou de présentation. Le navigateur les interprète et construit lui-même l'affichage.

C'est pour cette raison qu'un même site peut s'adapter à différentes tailles d'écran et qu'il est possible d'interagir avec ses éléments.

Cette idée sera importante lorsque vous écrirez votre premier fichier HTML : vous ne dessinerez pas directement les pixels de la page, vous décrirez sa structure.

---

## Slide 22 — Le même Web sur des machines très différentes

Un téléphone, une tablette, un ordinateur portable ou un téléviseur peuvent consulter le même site parce qu'ils utilisent des standards communs.

Le serveur n'a pas besoin de connaître exactement le matériel de chaque utilisateur pour envoyer un document HTML standard. Le navigateur se charge ensuite de l'interpréter.

Cette standardisation est l'une des forces du Web : elle permet à des machines très différentes de communiquer à partir de règles publiques partagées.

**Visuel suggéré :** même site affiché sur smartphone, tablette et ordinateur.

---

## Slide 23 — Le Web repose sur des couches invisibles

Lorsque vous consultez une page, vous voyez son contenu mais pas les nombreuses couches techniques situées derrière : réseau local, accès Internet, adressage, DNS, routage, protocole HTTP, serveur, HTML et navigateur.

Un problème sur une seule de ces couches peut empêcher l'affichage.

C'est pourquoi un informaticien cherche à localiser le niveau où se situe une panne plutôt qu'à conclure immédiatement que « Internet ne marche pas ».

**Exemple :** si un site précis ne répond pas mais que tous les autres fonctionnent, la connexion Internet entière n'est probablement pas coupée.

---

## Slide 24 — À retenir : de l'utilisateur au serveur

Internet est l'infrastructure mondiale reliant des réseaux. Le Web est un service qui fonctionne grâce à cette infrastructure. Le navigateur joue le rôle de client ; il demande des ressources à des serveurs Web selon un mécanisme de requête et de réponse.

Une consultation peut être résumée ainsi : **utilisateur → navigateur → DNS et réseau → serveur → réponse → navigateur → affichage**.

Dans la suite, nous allons ouvrir cette « boîte noire » et étudier plus précisément l'histoire de ces technologies, puis les rôles des adresses IP, du DNS, des URL et de HTTP.

**Visuel suggéré :** schéma final reprenant toute la chaîne avec des flèches dans les deux sens.
