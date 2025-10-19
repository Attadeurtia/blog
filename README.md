# Mon Blog Hugo

[![Hugo](https://img.shields.io/badge/Powered%20by-Hugo-blue.svg)](https://gohugo.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Bienvenue sur le dépôt de mon blog personnel, généré avec [Hugo](https://gohugo.io/), un générateur de sites statiques rapide et moderne.

---

## 📌 À propos

Ce dépôt contient le code source et le contenu de mon blog. Le site est construit avec Hugo et déployé automatiquement à chaque mise à jour.

**URL du blog :** [blog.cactuserveur.fr](https://blog.cactuserveur.fr)

Ce dépôt contient le code source et le contenu de mon blog. J'utilise le thème [Archie](https://github.com/athul/archie) que je modifie pour répondre à mes besoins, avec une traduction en français en cours.

---

## 🔄 Déploiement

Le site est automatiquement déployé via GitHub Pages à chaque push sur la branche main avec un nom de domain custom.

Pour générer le site en production J'utilise cette commande :

```bash
hugo --minify --gc
```

- minify : Minifie les fichiers HTML, CSS et JS pour optimiser les performances.
- gc : Active le ramasse-miettes (Garbage Collector) pour supprimer les fichiers inutilisés dans public/ (par exemple, les anciens articles ou images supprimés du contenu).
