---
title: "Comment configurer github"
date: 2023-04-27T17:49:47+02:00
draft: false
tags: ["git", "cheat-sheet","linux"] 
---

Pour utiliser github sur son ordinateur il faut installer git, ajouter une clé ssh dans son compte github et configurer git, puis télécharger le projet, ces étapes sont indispensables sur chaque machine.

## Installer git

Vérifier si git est déjà installé : `git --version` sinon [télécharger git](https://git-scm.com/downloads)

## Configurer git en local

C'est les informations qui seront affichées dans les commits, il faut les configurer une fois par machine.

- Configurer le nom d'utilisateur : `git config --global user.name "John Doe"`
- Configurer l'adresse mail :`git config --global user.email`

Les informations sont stockées dans le fichier `~/.gitconf`, si vous voulez les modifier vous pouvez le faire directement dans le fichier.

En soi, vous pouvez mettre ce que vous voulez, ce n'est pas lié à votre compte github, c'est juste pour que les commits soient plus clairs. Mais il est conseillé de mettre les mêmes informations que sur votre compte github.

## Générer une clé ssh

Il n'y a besoin que d'une clé ssh par machine, si vous avez déjà une clé ssh, vous pouvez la réutiliser, pour afficher votre clé ssh publique, vous pouvez utiliser la commande `cat ~/.ssh/id_rsa.pub`.

Si vous n'avez pas de clé ssh, vous pouvez [générer une clé ssh](https://www.linuxtricks.fr/wiki/wiki.php?id_contents=168) avec cette commande `ssh-keygen`, puis appuyer sur entrée pour valider tous les paramètres par défaut.

```bash
root@b99ab948939e:/# ssh-keygen 
Generating public/private rsa key pair.
Enter file in which to save the key (/root/.ssh/id_rsa): 
Created directory '/root/.ssh'.
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /root/.ssh/id_rsa
Your public key has been saved in /root/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:duhA+0K3IXdKJsyMFHu17v41E8+sEFIhe2cq++W8mas root@b99ab948939e
The key's randomart image is:
+---[RSA 3072]----+
|    .   o .      |
|     o . + .     |
|    o o o o o    |
|   . B o + +     |
|    . X S = .    |
|     . & X . =   |
|      . B . = +  |
|       o . * *   |
|        ..E.Oo   |
+----[SHA256]-----+
root@b99ab948939e:/#
```

Si cela ne fonctionne pas, il est possible que vous n'ayez pas installé ssh, pour l'installer : `sudo apt install ssh`.

Cela va créer deux fichiers dans le répertoire `~/.ssh` :`id_rsa` et`id_rsa.pub`. Le premier est la clé privée qui est à garder absolument secrète, le second est la clé publique, qui est à partager avec les différents services, ici github.

Puis vous pouvez copier coller votre clé ssh publique `cat ~/.ssh/id_rsa.pub`.

## Rajouter sa clé ssh à github

Maintenant, vous devez ajouter votre clé ssh publique à votre compte [github](https://docs.github.com/fr/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account?tool=webui).

## Télécharger le projet

Ne reste plus qu'à télécharger votre projet, sur la page du projet, cliquer sur le bouton vert "code" et copier le lien ssh, (attention, il faut bien copier le lien ssh et pas le lien https).

`git clone lien_ssh`

Voilà, vous pouvez commencer à travailler sur le projet, et les push seront directement envoyés sur le projet github.
