---
title: "Complexite"
date: 2023-04-28T14:18:49+02:00
draft: flase
tags: ["complexite", "cours"]
---


## Classes de complexité

|     | Déterministe | non-Déterministe |
| --- | --- | --- |
| temps | p,EXPTIME | np, NEXPTIME |
| espace | LOGSPACE, PSPACE, EXPSPACE | NLOGSPACE |

## complexité logarithmique

- O(1) : constant
- O(n) : linéaire
- O(log n) : logarithmique
- O(n log n) : quasi-linéaire
- O(n²) : quadratique
- O(n³) : cubique
- O(n^k) : polynomial
- O(2ⁿ) : exponentielle
- O(n!) : factorielle

![Capture d’écran du 2023-04-28 13-41-53.png](file://../) ![Capture d’écran du 2023-04-02 18-18-41.png](file:///Users/attadeurtia/.config/joplin-desktop/profile-2znq7d41/resources/50ddfc88bc5d49eaa791be3b071903c4.png)

|     |     | algo |
| --- | --- | --- |
| constant | O(1) | set |
| logarithmique | O(log n) | liste |
| linéaire | O(n) | recherche dichotomique, dans un tableaux trié |
| quasi-linéaire | O(n log n) | tri d'un tableaux (fusion) |
| quadratique | O(n²) | tri d'un tableaux (insertion) |
| cubique | O(n³) | multiplication de matrices |
| polynomial | O(n^k) |     |
| exponentielle | O(2ⁿ) | problème du sac à dos |
| factorielle | O(n!) | problème du voyageur de commerce |

## Problème complexe

### Problème du voyageur de commerce

- problème NP-complet
- O(n!)
- 10 villes : 3 628 800

### Problème du sac à dos

knapack problem

- problème NP-complet
- O(2ⁿ)
- 20 objets : 1 048 576

### Problème du plus court chemin

aussi appelé longest common subsequence

- problème NP-complet
- O(n²)
- 100 villes : 10 000

### Stable marriage problem

aussi appelé problème des mariages stables (stable matching problem) ou problème des épouses de Gale et Shapley (Gale–Shapley algorithm)

- problème NP-complet
- O(n²)
- 100 personnes : 10 000

Alago 1 : Gape-Shapley O(n²)

### vertex cover

aussi appelé couverture par sommets

Algo 1 : brute force O(2ⁿ)

#### glouton

Algo 2 : approximation O(n)
Algo 3 : heuristique du degré O(n²)

### clique

Algo 1 : brute force O(2ⁿ)
Algo 2 : approximation O(n)

### independent set

Algo 1 : brute force O(2ⁿ)
Algo 2 : approximation O(n)

### modularité

Algo 1 : brute force O(2ⁿ)
Algo 2 : approximation O(n)

### manathan distance

Algo 1 : brute force O(n²)

## heuriqtique

- 2-approximation
- degree

| Problème d'optimisation | Problème de décision |
| --- | --- |
| meilleur solution | oui/non |
| np-complet | np-difficile |
