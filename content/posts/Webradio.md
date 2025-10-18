---
title: "Webradio"
date: 2021-04-18T13:19:05+02:00
draft: false
tags: ["webradio", "vrac"]

---

## Pourquoi écouter la radio ?

Le terme radio ne fait pas rêver en 2021, de nos jours les platformes de streaming comme Deezer ou Spotify sont la norme pour écouter de la musique, pour les podcasts il existe des services comme podcast addict ou google podcast. Et devoir être limité par un flux constant dans lequel on ne peut pas choisir la musique, on ne peut pas mettre sur pause, et où l’on doit écouter à certaine heure pour écouter les émissions que l’on veut peut sembler absurde.
pourtant la radio possède encore de vrai argument.

- petit point explication
- avantage
- conseil de radio
- logiciel à utiliser

Déjà il faut faire la différence entre webradio et radio. Les radios normales qui existent toujours évoluent encore avec un gros changement de protocole l’année dernière. Les radios traditionnels fonctionnent par onde radio et son indépendante d’internet mais possèdent généralement une mauvaise qualité audio, contrairement au radio web qui comme le nom le suggère, fonctionne via internet. Avant souvent lié au radio pirate, les webradios sont maintenant bien répandus, avec la majorité des radios traditionnelles possédant leurs versions http.

## Les avantages

Premièrement et pas des moindres, le **coût**, ça peut sembler étrange à une époque où le moindre service se transforme en abonnement payant mais les webradios fonctionnant via un standard libre sont totalement gratuites et sans pub, de plus certaines offres une qualité audio au niveau d’un CD, soit une option souvent chère sur les services de streaming quand ce n’est tout simplement pas disponible. Et ça 24/24 et sur n’importe quel appareil pour peu qu’il puisse se connecter au web.

Comme souligné précédemment, elles fonctionnent toutes sur le même standard libre, ce qui leur permet d’être géré de la même façon sur n’importe que quelle device. De plus le standard permet d’afficher en temps réel le titre de la musique ou bien le nom de l’émission en cours ce qui permet dans une certaine mesure de compenser l’absence du bouton playlist des plateformes de Streaming. Évidemment ça ne permet pas directement de pouvoir réécouter une musique relevée qui serait enregistrée dans les coups de cœur, mais avec un système d’automatisation assez basique il est possible de télécharger la musique directement sur YouTube.

Autre net avantage, l’absence totale de tracking. Ici pas de question de vie privée, ou de vol de données car n’y en a tout simplement pas. Tu récupères l’URL du flux audio et c’est tout. Et mine de rien, un service gratuit et qui ne se sert pas des données utilisateurs pour vivre c’est assez rare.

Autre point qui découle directement du précédent, il n’y a pas de « flow » ou autres playliste personnalisée selon l’utilisateur. Mais là où certain y voie un frein, j’y vois un net avantage, déjà je n’ai jamais été frillant du flow, je l’ai toujours trouvé merdique, que ce soit sur Deezer que j’ai utilisé pendant 5 ans et qui est donc sensé bien me connaitre, ou Spotify cador du marché.Je m’explique, souvent il me mettait dans une boucle de musique composée soit de toujours les mêmes morceaux et parce que je les réécoutais il me les reproposait a chaque nouveau lancement du flow, soit il me proposait les morceaux les plus connus d’un genre ou d’un artiste, et donc souvent les mêmes.
Alors que là, le net avantage d’une radio c’est que le seul paramètre que l’a choisis c’est le genre que l’on veux écouter, le plus souvent les radios ont un thème général et passent des musiques liées, je prends l’exemple de la super radio Fip, il y a une déclinaison Fip rock, Fip Jazz, Fip musique du monde… du coup quand j’ai envie d’écouter plutôt du rock, je vais sur une radio rock, quand je veux un peu de nouveauté je passe sur une radio musique actuelle. Et c’est beaucoup plus riche que n’importe quelle flow, le nombre de pépites que j’ai découvert depuis que j’écoute Fip m’a clairement fait oublier le flow. ça offre vraiment de nouvelle opportunité de découvert, à tous les gens qui disent que la musique c’était mieux avant, faites leurs écouté Fip musique nouveauté ou bien radioalpa, et ils verront (s’ils ne sont pas de mauvaise foi, malheureusement c’est assez rare) que les talents actuels sont bien plus larges que la soupe fade que nous proposent les médias mainstream.

- coût gratuit
- sans pub
- haute qualité
- standard libre
- disponible partout pareil
- Absence de traçage
- découvert et nouveauté

## Les radios existantes

passons maintenant à la pratique, comment récupérer ce fameux flux radio ? déjà ça fonctionne comme adresse http souvent de la forme : http://www.radioalpa.com:8000/live avec le nom de domaine du site et mp3, flac ou aac comme extension. L’adresse du flux étant assez compliqué a récupérer, je vous passe l’adresse d’un tuto : [Astuce : Récupérer le flux HTTP d’une webradio !](https://www.youtube.com/watch?v=u85jS1SPt10), et des bases de données qui en liste plusieurs : 

- [http://radiobit.50webs.com](http://radiobit.50webs.com/)
- http://forum-hifi.fr/thread-18229.html
- https://community.roonlabs.com/t/internet-radio-flac-stations-swap-meet/42327

Parmi mes coups de coeur, il y a tout d’abord Radioalpa, une radio local du Maine, qui passe des musiques indé et modernes et de super émissions très varié, ça va d’une émission sur le genre, à la carotte, souvent parsemé de points info. en somme une radio très complète.

- **RadioAlpa** : http://www.radioalpa.com:8000/;&type=mp3

il y a aussi tout la série de FIP radio avec ses déclinaisons de tous genres qui passent de la musique sans interruption toute la journée, excepter sur FIP normal qui se permet des émissions musicales le soir.
Le seul point négatif c’est qu’ils ne précisent pas la musique en cours dans les data données, ce qui oblige de se référer au site pour les titres.

- **FIP** : http://icecast.radiofrance.fr/fip-hifi.aac
- FIP **rock** : http://icecast.radiofrance.fr/fiprock-hifi.aac
- FIP **groove** : http://icecast.radiofrance.fr/fipgroove-hifi.aac
- FIP **pop**: http://icecast.radiofrance.fr/fippop-hifi.aac
- FIP **electro** : http://icecast.radiofrance.fr/fipelectro-hifi.aac
- FIP **musique du monde** : http://icecast.radiofrance.fr/fipworld-hifi.aac
- FIP **reggae** : http://icecast.radiofrance.fr/fipreggae-hifi.aac
- FIP **nouveauté** : http://icecast.radiofrance.fr/fipnouveautes-hifi.aac
- FIP **jazz** : http://icecast.radiofrance.fr/fipjazz-hifi.aac

Avec FIP on couvre déjà une bonne partie du spectre musical mais il me manquait encore des genres, notamment un très populaire en ce moment : la K-pop, c’est presque par hasard que je suis tombé sur ce site très bien fait : [listen.moe](https://listen.moe/) qui propose même des bots discords, une application android franchement bien faite et la liste des morceaux précédemment passé.

- **j-POP** : https://listen.moe/stream
- **k-POP** : https://listen.moe/kpop/stream

Pour finir, une radio passant que des OST de films, parfait pour travailler.
Après quelques recherches, je trouve [La grande Évasion](https://www.lagrandeevasion.fr/), zéro interruptions, que de la musique de flims h24:

- musique de film : http://radio.lagrandeevasion.fr/evasion.mp3

La liste n’est pas exhaustive, il manque par exemple du classique/ baroque que je préfère écouter en CD ou bien du rap pour lequel je suis trop assez sélectif pour l’écouter en radio.

En vrac quelques propositions :

- **rock haute qualité** : https://stream.radioparadise.com/rock-flac
- **classique** : http://rondo.iradio.fi:8000/klasupro.flac
- **indé** : http://91.121.159.124:8000/eko-des-garrigues-256k.ogg

## Les logiciels

il est important pour un service de musique d’être réactif et facile d’accès, d’avoir des raccourcis et d’être reconnus comme source audio pour mettre sur play/pause depuis n’importe quelle interface 

sur Linux il y a l’extension gnome « [radio](https://extensions.gnome.org/extension/1247/gnome-radio/) » qui est très bien intégré et surtout simpliste, on peut choisir le flux, le volume et play/pause, en plus on peut copier le nom du titre en cours directement dans le presse papier. Simple efficace, je voixs pas trop ce que l’on peut faire de mieux, sur Windows VLC le gère basiquement la radio, sinon pas mal de logiciels dédiés existent. Sur Android, il y a [PodcastAddict](https://play.google.com/store/apps/details?id=com.bambuna.podcastaddict&hl=fr&gl=US), véritable couteau suisse de l’audio sur android, il permet d’écouter des podcasts, n’importe quelle fichier son, et les radios, il possède également de nombreux raccourcis et widget, à l’opposé il y a [transistor](https://play.google.com/store/apps/details?id=org.y20k.transistor&hl=fr&gl=US). Open-source il ne sert qu’a la radio mais il le fait bien, l’interface est très claire, beaucoup moins bordélique que PodcastAddict, elle va au direct.

j’espère avoir couvert avec ce billet tous les aspects des webradios et vous avoir donné envie d’en essayer.
