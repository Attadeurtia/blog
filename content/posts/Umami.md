+++
date = '2025-02-15T18:30:17+01:00'
draft = false
title = 'Comment Installer Hugo Umami Analytics Module'
+++

## Qu'est-ce que Umami ?

[Umami](https://umami.is) est une alternative open-source à Google Analytics, il faut savoir que Google Analytics [ne respecte pas le RGPD](https://agence-anode.fr/blog/google-analytics-4-rgpd-conformite-enjeux-alternatives/) et tous les sites l'utilisant en France et en Europe sont dans l'illégalité vis-à-vis des données personnelles.

Umami à l'inverse est conçue pour respecter la vie privée des utilisateurs tout en fournissant des statistiques utiles sur l'utilisation de votre site. Il existe d'autre alternative, mais celle-ci est facile à mettre en place et possède un hugomod.

## Prérequis

Avant de commencer, assurez-vous d'avoir les éléments suivants :

1.  **Hugo installé** : Vous pouvez télécharger Hugo depuis [le site officiel](https://gohugo.io/getting-started/installing/).
2.  **Un projet Hugo existant** : Si vous n'avez pas encore de projet, vous pouvez en créer un avec la commande `hugo new site mon-site`.
3.  Go installé sur votre machine

## Étapes pour Installer un Mod

### 1\. Initialiser un Module Hugo

Si ce n'est pas déjà fait, initialisez votre projet Hugo comme un module. Dans le répertoire de votre projet, exécutez :

```bash
hugo mod init github.com/votre-utilisateur/votre-projet
```

Cela va créer un fichier `go.mod` que vous n'avez pas besoin de toucher.

### 2\. Ajouter umami-analytics

On va utiliser [ce mod là](https://hugomods.com/analytics/umami/) pour installer Umami sur notre site Hugo, cela fonctionne notamment avec Githubpage (qui héberge cette page).

Vous pouvez ensuite rajouter ceci dans le fichier `hugo.toml` (ou dans le fichier `config.toml`).

```
[module]
  [[module.imports]]
    path = 'github.com/hugomods/umami-analytics'

[params]
  [params.services]
    [params.services.umami_analytics]
      id = 'XXXXXXXX'
      script_url = 'https://cloud.umami.is/script.js'

```

Cela va télécharger automatiquement le module.  
Pensez bien à remplacer `XXXXXXXX` par l'id correspondant que vous trouverez sur votre compte Umami.

### 3\. Configurer le Mod

Une fois le mod ajouté, vous devez l’activer dans le head de votre site comme sur n'importe quel autre projet, pour cela rendez-vous dans `Layout/partials/head.html` et copier cette ligne dedans. Si le fichier n'existe pas, vous devez le créer le suivant le même chemin.

```
<head>
  {{ partialCached "hugomods/umami-analytics/index" . .Params.analyze }}
</head>
```

Attention à bien le faire dans `layouts/partials/head.html` et non dans `themes/Layout/partials/head.html`, normalement vous n'aurez jamais à modifier le dossier thème.

Il est possible que selon le thème, `partials/head.html` porte un autre nom, ou soit autre part. Si c'est le cas, référez-vous à la doc de votre thème.

### 5\. Tester votre Site

Pour vérifier que tout fonctionne correctement, mettez en ligne votre site. Ouvrez la console (F12) sur la page et allez dans Réseau, puis filtrez par "umami" et recharger la page, (crt+R) vous devriez le voir apparaitre, vous pouvez également voir une ligne similaire dans Éléments : `<script defer="" src="https://cloud.umami.is/script.js" data-website-id="XXXXXXXXXX"></script>` dans le head.

Si cela n'apparait pas c'est que le fichier `head.html` est au mauvais endroit ou mal nommé.

Si cela apparait comme bloqué c'est que vous avez des extensions de protection de vie privée, désactivez les pour votre site ou tester le sur un autre navigateur, cela devrait fonctionner.

### 6\. Tester votre Site

Voilà, vous pouvez maintenant voir  le trafic sur votre site via Umami.  
https://eu.umami.is/share/zzfs09Ge7qh5YIHX/attadeurtia.github.io