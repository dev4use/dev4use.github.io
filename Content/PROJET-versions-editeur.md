# Plusieurs versions de la solution

Pourquoi ne pas entretenir et maintenir plusieurs versions de la solution ?  
Exercice de style intéressant et maîtrise précise des périmètres fonctionnels.  

## Maîtrise du périmètre fonctionnel

Il est si facile de s'égarer, d'aller trop loin, de tomber dans le gadget et le superflu.  
Mais il est aussi si tentant d'avoir un objet technologique qui élargit sans cesse son périmètre.  
 > Il en faudrait donc pour tous les goûts ?  

D'où la gestion en parallèle de plusieurs versions.    

## Panel d'offre

La progressivité de l'offre se décline en trois niveaux. 

- Standard
- Premium
- Optimum

## Approches produit différentes

Il ne s'agit pas tant de décliner une logique commerciale que de mesurer la progressivité de l'offre et que de maintenir la pluralité de l'offre :

- MVP (Minium Viable Product)
- MMP (Minimum Marketable Product)
- product (sous entendu final et idéal)

A tout moment il faut pouvoir maintenir ou enrichir une version minimum.  
Cette version réduite est réputée stable et peut servir de repli en cas de bug majeur avec retour arrière difficile sur une version usine à gaz buggée.  

## Approche qualité

Pour preuve que même la version Standard de <a href="https://github.com/dev4use/marss" class="trademark">Marss</a> n'est pas délaissée, toute [version officielle du produit](PROJET-versioning.md) respecte **une barrière de qualité** avant publication.

Toute version majeure du produit, de niveau de numérotation 1 sur 3, respecte donc les règles suivantes (que je sais contestables mais dont je m'amuse) :

1. Couverture du code par les tests à 100 %.
1. Tests à 100 % OK.
1. 0 violation de convention de codage (léger ajustement et sans excès sur la taille des lignes).
1. Documentation de code source actualisée et lisible.
