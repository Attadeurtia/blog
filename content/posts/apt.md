---
title: "Apt"
date: 2023-04-23T22:03:54+02:00
draft: false
---

# apt

Voici les commandes les plus couramment utilisées avec `apt` :

- `sudo apt update` : Mettre à jour la liste des paquets disponibles
- `sudo apt upgrade` : Mettre à jour tous les paquets installés
  - `sudo apt upgrade -y`
- `sudo apt install <nom_du_paquet_1> <nom_du_paquet_2>`  : Installer un paquet
- `sudo apt remove <nom_du_paquet>` : Supprimer un paquet
- `sudo apt search <terme_de_recherche>` : Rechercher un paquet
- `sudo apt autoremove` : Supprimer les paquets qui ne sont plus nécessaires
- `sudo apt clean` : Supprimer les fichiers de cache téléchargés lors de l'installation de paquets
- `apt clean` efface tout du répertoire local des fichiers de paquets récupérés. Il supprime tout sauf le fichier de verrouillage de `/var/cache/apt/archives/` et `/var/cache/apt/archives/partial/`¹.
- `apt autoclean`, comme `clean`, efface le répertoire local des fichiers de paquets récupérés. La différence est qu'il ne supprime que les fichiers de paquets qui ne peuvent plus être téléchargés et qui sont en grande partie inutiles. Cela permet de maintenir un cache sur une longue période sans qu'il ne devienne incontrôlable¹.
- Il n'y a pas d'option `clear` pour la commande `apt`.

(1) apt - What is difference between the options "autoclean", "autoremove .... [https://askubuntu.com/questions/3167/what-is-difference-between-the-options-autoclean-autoremove-and-clean](https://askubuntu.com/questions/3167/what-is-difference-between-the-options-autoclean-autoremove-and-clean).
(2) apt - clean, autoclean, and autoremove --- combining them is a good .... [https://askubuntu.com/questions/984797/clean-autoclean-and-autoremove-combining-them-is-a-good-step](https://askubuntu.com/questions/984797/clean-autoclean-and-autoremove-combining-them-is-a-good-step).
(3) Difference between apt clean & apt autoclean in Ubuntu. [https://techpiezo.com/linux/difference-between-apt-clean-apt-autoclean-in-ubuntu/](https://techpiezo.com/linux/difference-between-apt-clean-apt-autoclean-in-ubuntu/).
(4) linux - What are the differences between apt clean/remove/purge etc .... [https://stackoverflow.com/questions/68635646/what-are-the-differences-between-apt-clean-remove-purge-etc-commands](https://stackoverflow.com/questions/68635646/what-are-the-differences-between-apt-clean-remove-purge-etc-commands).
