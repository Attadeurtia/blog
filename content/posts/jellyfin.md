---
title: "Bonne utilisation de Jellyfin"
date: 2024-03-22T14:52:41+01:00
draft: false
---

# Pourquoi vaut-il mieux installer l’application que d’utiliser le navigateur ?
Il est recommandé d’utiliser l’application officielle de Jellyfin plutôt que le navigateur, car les films utilisent [les codecs](https://fr.wikipedia.org/wiki/Codec) H.264 (AVC) ou H.265 (HEVC). [Les navigateurs](https://jellyfin.org/docs/general/clients/codec-support/) ne prennent en charge que le H.264, ce qui oblige le serveur à convertir le format (transcodage) des films HEVC, ce qui consomme plus de 90 % des ressources du serveur.

La moitié des films de la bibliothèque sont en H.265 : d’une part, c’est un [format mieux adapté](https://www.tomshardware.com/reference/h264-h265-hevc-codec-definition) et plus moderne, mais également plus léger et esthétique que le H.264. La solution la plus optimisée est donc d’installer l’application officielle.

# Comment installer l’application Jellyfin
- Application Android officielle : [Google Play](https://play.google.com/store/apps/details?id=org.jellyfin.mobile)
- Application Android que j’utilise : [Jellyfin pour Android (JDTech)](https://play.google.com/store/apps/details?id=dev.jdtech.jellyfin)
- Application Windows officielle : [Jellyfin Media Player (GitHub)](https://github.com/jellyfin/jellyfin-media-player/releases)
![Version de Windows à télécharger sur GitHub](/images/jellyfin.md/Version_de_Windows.png)
*Attention à bien prendre la version x64 et non la x86.*

[Lien officiel de toutes les versions de Jellyfin](https://jellyfin.org/downloads)

---

**Remarque** : si le film est en H.264, vous pouvez le lire depuis le navigateur sans souci.

**Film en H.264 (AVC)**
![Film en H.264 (AVC)](:/f481bec57ac6480ab8e1c06e9d87d4f3)

**Film en H.265 (HEVC)**
![Film en H.265 (HEVC)](:/17617e536ec64a28815b068a77c0bf6e)

---

**Note** : Windows ne gère pas non plus nativement le H.265, mais vous pouvez télécharger [VLC](https://www.videolan.org/vlc/) pour le lire (si ce n’est pas déjà fait, il a quand même été installé plus de 400 milliards de fois).
