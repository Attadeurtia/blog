---
title: "Comment Devenir Invisible Sur Internet"
date: 2022-06-30T20:54:24+02:00
draft: false
tags: ["open-source", "vrac"]
summary: "Comment devenir invisible sur internet ? Comment protéger sa vie privée sur internet ? Comment être anonyme sur internet ?"
---

Cet article va essayer de condenser tout ce qu’il faut savoir ou mettre en place pour améliorer sa vie privée sur internet, j’ai essayé de le faire tout public mais si vous avez une question ou une remarque n’hésitez pas à me contacter.

<!--more-->

![image d'illustration](/Comment_Devenir_Invisible_Sur_Internet/b57adf14ba4b4d68949d83a9ebf14d26.png)

## Pourquoi être invisible sur internet ?

<https://lecrabeinfo.net/pourquoi-proteger-sa-vie-privee-sur-internet.html>

Avez-vous vu le film Snowden ? Sinon allez le rattraper immédiatement, mais pour faire simple Edward Snowden, lanceur d’alerte dévoile au grand monde comment la NSA applique depuis les attentats des tours jumelles une surveillance de masse implacable sur la population mondiale. Et si les méthodes vues dans le film vous effraie, dites-vous que c’était il y a 10 ans et que maintenant c’est sûrement bien pire.

Je vais donner quelques exemples concrets : vous prévoyez une action écologique, légale ou non, pacifiste ou non, vous devez faire attention car vous allez être surveillés et fichés.
Vous faites des recherches sur des sujets sensibles juste pour votre culture, ou par curiosité comme sur les armes, ou la drogue, vous pouvez être fichés.
Préjudice, comme pour Hong Kong qui est passé d’une ville libre à la dictature chinoise et dont le passé des gens à une époque où certaines choses étaient légale maintenant nuie à leur vie actuelle sous le régime chinois.

Cela permet aussi d’échapper dans une toute autre mesure aux bulles de filtres sur internet qui nous enferment dans certaines cases et centres d’interêt voici un article sur les bulles de [filtre de bulle de google](https://spreadprivacy.com/google-filter-bubble-study/).

Plus généralement, c’est important de savoir comment faire, au cas où un jour vous aurez des informations compromettantes à diffuser, et puis c’est une bonne hygiène informatique à avoir. Ne serait-ce que pour arrêter de donner des informations personnelles aux grandes entreprises et ainsi arrêter de participer à la publicité de masse.

Aussi, simplement parce que la grande partie des étapes ci-dessous ne vont pas impacter votre qualité de navigation sur internet et même potentiellement la rendre plus rapide.

## À la base

La base pour être invisible sur internet est le chiffrement (cryptage en anglais), ce procédé permet de brouiller le message entre deux parties, pour que toute interception de l’information soit totalement illisible. Dès que vous pouvez mettre en place une connexion chiffrée, que ce soit en navigation web en mail, ou en discussion avec les autres, privilégiez toujours les solutions chiffrées.

Petit point, il faut savoir que vos appels et vos SMS de base ne sont pas chiffrés, cela signifie qu’ils voyagent en clair sur le réseau. Si quelqu’un ou un organisme décide de l’intercepter, il peut lire ou écouter directement ledit message, il lui suffit de créer une antenne qui simulera le réseau 4G à laquelle votre téléphone va se connecter automatiquement, pour récupérer ses informations en claire de vos conversations.

Notez qu’il n’est pas nécessaire d’être totalement invisible sur internet mais juste assez par rapport à la surveillance dont vous faites preuves, à moins que vous ne soyez un activiste activement recherché, simplement les étapes de ce guide suffisent amplement.

- Faites le points
- Navigateur
- Moteur de rechercher
- Extension
- DNS
- Proxy
- VPN
- Tor
- Messagerie
- Extrême

## Faites le point

Déjà, il faut savoir que même si vous ne faites pas tout ce qui est indiqué, ce n’est pas grave et il y aura quand même un gain. L’objectif est surtout de vous renseigner et de vous ouvrir les yeux. Mais le plus important c’est que vous vous sentiez à l’aise avec votre matériel et votre utilisation .

Cet article est construit par ordre de facilité, les changements les plus simples sont au début de façon croissante, c’est-à-dire que les 3/4 premières étapes peuvent être faites par tout le monde sans trop de difficulté en quelques minutes.

Pour vérifier si vous êtes plus ou moins sécurisés, vous pouvez aller sur le site de mullvad qui vous indique si votre DNS a des fuites ou si votre ip est blacklisté <https://mullvad.net/fr/check/>
ou alors [https://amiunique.org](https://amiunique.org/) qui vous indique si vous êtes un profil unique, plus vous êtes unique, plus il est facile de vous suivre sur internet.

Le plus simple pour commencer est de changer son moteur de recherche, on peut faire ça facilement sur tous les périphériques se connectant à internet.

## Navigateur

Petit point sur la différence entre navigateur et moteur de recherche, le navigateur est l’application que vous utilisez pour aller sur internet, typiquement Chrome, Edge ou Firefox, tandis que le moteur de rechercher est le site internet qui vous permet de faire une recherche sur internet par défaut, Google, Bing, Ecosia. Mais les sites comme Wikipédia possèdent aussi leurs propres moteurs de recherche internes qui permettent de faire une recherche sur leur site «  insérer URL ».

Vous pouvez commencer par bannir les navigateurs des gafam, dégagez Chrome, Edge, Safari et Consorts, ce sont de véritable puits d’informations, et privilégiez des alternatives libres, ça va revenir souvent dans ce billet mais c’est souvent bien mieux pour votre vie privée d’utiliser des applications libres et open source que les autres. Pour cela, je vous conseille le très célèbre [Firefox](https://www.mozilla.org/fr/) qui est rapide, moderne et fonctionne très bien aussi bien sur ordinateur que smartphone.

Si vous voulez rester sur la même base que Chrome et utiliser les mêmes extensions, il existe [Chromium](https://www.chromium.org/Home/) (à ne pas confondre car ce dernier est open source).

À titre personnel j’utilise [Vivaldi](https://vivaldi.com/fr/), qui n’est pas libre mais ne stocke pas vos informations personnelles. Il est plein d’options, comme gestionnaire de mots de passe, note synchronisée en ligne, lecteur de flux RSS et plein d’autres choses. Typiquement, mon blog est hébergé chez eux.

Dans Firefox (ou autres si vous avez installé autre chose) je vous conseille d’aller dans les réglages et d’activer le plus d’options liées à la vie privée. Faites juste attention à ne pas supprimer tout les cookies car ceux-ci enregistrent les mots de passes, donc à moins que vous ne vouliez vous reconnecter à chaque fois que vous allez sur un site, il vaut mieux les laisser activés.

![Les parametres dans Firefox](/Comment_Devenir_Invisible_Sur_Internet/6168c1578a3748e0a7858dea515eb4b1.png)

## Moteur de recherche

Quand vous avez installé Firefox, il faut donc choisir un moteur de rechercher, là encore évitez comme la peste les gafam, c’est-à-dire **Google** notamment, mais favorisez [Ecosia](https://www.ecosia.org/) ou [Lilo](https://www.lilo.org/) (moteurs de recherche écolos), le plus efficace à mes yeux c’est [Duckduckgo](https://duckduckgo.com/), je le trouve même plus pertinent que Google.
Sinon, sur mon PC j’utilise [Startpage](https://www.startpage.com/), c’est un moteur de recherche un peu particulier, sans collecte, suivi ou ciblage de données personnelles et d’ont l’anonymat est le fer de lance.[](https://www.startpage.com/fr/make-homepage/?t=dark)

![Changer le moteur de recherche dans Firefox](/Comment_Devenir_Invisible_Sur_Internet/f49cbcbce75143be9b5e3878e294f31b.png)

## Extensions

Une fois que vous avez votre navigateur mis en place, vous pouvez aussi installer des extensions pour vous supprimer automatiquement les traqueurs et autres ciblages. J’aime bien cette option car elle est extrêmement simple, [les extensions Chrome](https://chrome.google.com/webstore/category/extensions) et [Firefox](https://addons.mozilla.org/fr/firefox/) s’installent en un clic, vous pouvez les retrouver à ces adresses :
pour Chrome : <https://chrome.google.com/webstore/category/extensionspour> Firefox : [https://addons.mozilla.org/fr/firefox/](https://chrome.google.com/webstore/category/extensions)

![Les paramètres de privacy Badger](/Comment_Devenir_Invisible_Sur_Internet/a3923796b56e479b83ff32f66d3713a8.png)

Je conseille en premier lieu [Privacy Badger](https://privacybadger.org/), qui va bloquer le plus possible de traqueurs. Dans les paramètres de celui-ci, ajoutez l’option « Apprendre à bloquer les nouveaux traqueurs lors de la navigation »

Indispensable, installez aussi le classique [uBlock Origin](https://ublockorigin.com/fr) sans qui la navigation en ligne est infernale (il permet de bloquer un grand nombre de pub, surtout sur YouTube). N’utilisez plus Adblock Plus car il ne supprime qu’une partie des pubs en accord avec société publicitaire : un article qui en parle [http://bloquelapub.net](http://bloquelapub.net/).

Ces deux extensions existent aussi bien sur **ordinateur que sur téléphone.**

![Paramètres extentions Firefow](/Comment_Devenir_Invisible_Sur_Internet/a1eb6a9537424a43980f583351dd2cc7.png)
![Listes d'extentions pour mobiles](/Comment_Devenir_Invisible_Sur_Internet/37e660e8b14f47178ad463b74b9c2a42.jpg)

## DNS

Le serveur DNS est le premier service que vous utilisez lorsque vos faites une recherche en ligne.

Il faut voir ça comme les pages jaunes qui associent votre recherche au serveur web correspondant.
Chaque site est répertorié grâce à une adresse ip, c’est comme son adresse postale. Quand vous cherchez le service « YouTube » votre ordinateur va envoyer une requête à votre DNS pour savoir quelle est l’adresse ip du site YouTube et votre DNS va renvoyer quelque chose comme 94.130.212.178 à votre ordinateur qui va pouvoir contacter YouTube.

Changer de DNS va aussi permettre de filtrer une bonne partie des pubs en ne redirigeant pas la demande de publicité vers votre ordinateur.

Votre DNS (resolver) par défaut est celui de votre opérateur téléphonique (Orange, SFR…) ou celui de Google mais celui-ci surveille vos recherches et bloque même certains sites internet en fonction de la localisation.

Ça prend 2 secondes de changer ça dans vos paramètres. Pour Android c’est directement dans les paramètres « réseau et internet » et sur ordinateur je vous donne des ressources : <https://github.com/DNSCrypt/dnscrypt-proxy>.

- pour Windows : <https://lecrabeinfo.net/changer-les-dns-sur-windows-10.html>
- pour IOS : <https://www.01net.com/astuces/comment-modifier-son-dns-sur-iphone-et-ipad-1395559.html>

![Paramètres DNS sur Android1](/Comment_Devenir_Invisible_Sur_Internet/fdd9a1c5cfae46e1a071aaa54e7d22a1.png)
![Paramètres DNS sur Android2](/Comment_Devenir_Invisible_Sur_Internet/afa18a3dc3344a80bcdd2ab5f530d6f3.png)

Voici un très bon [article](https://sebsauvage.net/wiki/doku.php?id=dnsfilter) si vous voulez aller plus loin pour configurer votre DNS sur android personnalisé.

Si vous ne voulez pas vous prendre la tête, le DNS de Cloudfaire, leader dans le domaine d’ont l’adresse est : 1.1.1.1 et assure ne pas récupérer vos données. Sinon vous en avez des plus privés, voici [une liste](https://adguard-dns.io/kb/fr/general/dns-providers/), il vaut mieux privilégier les DNS en https ou TLS car ils sont chiffrés comme [adguard](https://adguard-dns.io/fr/welcome.htm) typiquement.

## Proxy

Un proxy est un serveur auquel on se connecte comme passerelle pour accéder à internet, ce qui signifie que les sites que vous visiterez verront les informations de ce serveur et non les vôtres directement. Vous pouvez en trouver beaucoup de gratuits, mais ils seront rarement chiffrés.

![Shéma fonctionnement de proxy](/Comment_Devenir_Invisible_Sur_Internet/7448c910d9144b1eaa44ee73b18d2966.png)

L’une des façons de vous identifier sur internet est via votre adresse ip, votre adresse ip est comme une adresse postale et permet d’identifier une personne. Passer par un proxy masque votre adresse ip car le site que vous visitez verra l’ip du serveur proxy et non la vôtre.

Vous pouvez mettre en place un proxy sur tout votre trafic internet de votre ordinateur/ smartphone, ou bien le mettre seulement pour certains services comme le mettre uniquement sur votre navigateur.

Vous pouvez en trouver beaucoup de gratuits, mais ils sont rarement chiffrés : <http://free-proxy.cz/fr/>.
Sinon vous avez ce services de proxy et vpn chiffrée [https://www.sslprivateproxy.com](https://www.sslprivateproxy.com/).

## VPN

Le VPN est simplement un type particulier de proxy. Vous connaissez sûrement globalement les VPN, mais l’une de leurs fonctions très utiles est que, comme toute votre connexion internet est chiffrée et va passer par un serveur tiers, ce n’est normalement pas possible pour un hacker ou les services de renseignements de revenir vers vous (bien sûr vous pouvez utiliser des VPN en cascade pour encore plus de sécurité mais je pose juste ça là).

Encore une fois le problème est de faire confiance au service que vous utilisez et sachez que vous ne pouvez jamais avoir de garantie qu’ils n’utilisent pas vos données personnelles (sauf si vous en montez un vous-même) mais le service de VPN contrairement au reste sont payants, monnayant 5e par mois. J’utilise [Mulvad](https://mullvad.net/fr/), qui est respectueux de la vie privée et assez versatile, ils ont une application Windows, Linux et Android pour ceux qui veulent quelque chose de simple, il peut aussi se configurer avec Openvpn, donc rien à dire de plus, il fonctionne bien et est simple.

## TOR

La dernière étape pour être sûr de ne pas être suivi est d’utiliser Tor Browser qui est un navigateur, disponible sur tous les appareils (sauf iPhone). Il permet d’être totalement intraçable sur le web, quand vos faites une recherche dessus. Chacune de vos requêtes passe par plusieurs proxys en étant chiffrée à chaque étape, avant d’atteindre la source, ce qui vous assure de ne pas être suivi. Attention seulement, Tor Browser supprime quelques fonctionnalités comme Javascript qui pourront permettre à un site de vous retrouver.

Notez que l’utilisation de Tor Browser n’est pas exclusive au deepweb mais s’utilise très bien de façon standard. Si vous voulez aller sur le deepweb par contre il vous faudra respecter deux trois autres règles que je ne détaillerai pas ici.

L’utilisation de Tor est une très bonne idée mais le réseau est un peu lent.

## Messagerie

Si vous voulez discuter avec quelqu’un de façon sécurisée sans que personne ne puisse intercepter votre discussion, je ne peux que vous conseiller [Signal](https://signal.org/fr/), et en mail chiffré il n’y a pas mieux que [Tutanota](https://tutanota.com/fr/) tout deux sont gratuits.

## Extreme

Pour les plus extrême d’entre vous, je vous conseille d’utiliser Qubes OS, une version de Linux basée sur la sécurité et l’anonymat. Bien sûr, si vous pouvez créé votre propre proxy c’est l’idéal car vous aurez la main mise dessus, et pour tout document vraiment sensible, manipulez les sur des ordinateurs qui ne sont pas et n’ont jamais été connectés à internet.

Pour résumer, personnellement j’utilise au quotidien Vivaldi sur mon ordi et mon téléphone avec DuckDuckGo et comme extension : privacy badger et Ublock, comme DNS j’utilise AdGuard et un custom sur andoid.
Occasionnellement, j’utilise le VPN fourni avec ma version d’Android : [/E/os,](https://e.foundation/e-os/) et Mullvad et de temps à autre j’utilise Tor pour faire deux trois recherches. Sinon, pour communiquer j’emploie au maximum signal.

## bonus

- <https://mullvad.net/fr/help/second-steps-toward-online-privacy/>
