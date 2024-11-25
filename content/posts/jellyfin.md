---
title: "Jellyfin"
date: 2024-03-22T14:52:41+01:00
draft: true
---

# Pourquoi il vaut mieux installer l'application que d'utiliser le navigateur ? 
Pour utiliser Jellyfin, le mieux est d'utiliser l’application officiel que le navigateur car les films sont codés soit en H.264(AVC) soit en H.265(HEVC), hors les [navigateurs](https://jellyfin.org/docs/general/clients/codec-support/) ne prennent en charge que le H.264, du coup le serveur doit convertir un format à l’autre (transcoder) mais cela lui prend trop de ressource (>90%).

La moitié des films de la bibliothèque étant en H.265 [car c’est mieux](https://www.tomshardware.com/reference/h264-h265-hevc-codec-definition), c'est un format plus moderne, plus léger, plus beau, la solution est d’installer l'application officielle car celle-ci gère nativement les deux codecs, et donc ne sature pas inutilement le serveur et le film reste fluide.
# Comment installer l'application Jellyfin
- Application Android officielle : https://play.google.com/store/apps/details?id=org.jellyfin.mobile
- Application Android que j'utilise : https://play.google.com/store/apps/details?id=dev.jdtech.jellyfin
- Application Windows officielle : https://github.com/jellyfin/jellyfin-media-player/releases

![version de Windows à téléchargé sur github](static/jellyfin/0cddccac91c94734806025ea28e898cb.png)
*Attention à bien prendre la version X64 et non la X86*
{{ $image := .Resources.Get "0cddccac91c94734806025ea28e898cb.jpg" }}

Lien officiel de toutes les versions de Jellyfin : https://jellyfin.org/downloads
* * *

Remarque, si le film est en H.264 vous pouvez le lire depuis le navigateur sans souci.

Film en H.264 (HEVC)
![Film en H.264 (HEVC)
](:/f81631931bb849c4b4c437e2d2bc3f2f)

Film en H.265
![Film en H.265
](:/e6d8006348bd4b6db0752c837467ef24)
* * *

Note : Windows ne gère pas non plus nativement le H.265, mais vous pouvez télécharger [VLC](https://www.videolan.org/vlc/) pour le lire (si ce n'est pas déjà fait, il a quand mêmé été installé plus de 400 milliards de fois).  
