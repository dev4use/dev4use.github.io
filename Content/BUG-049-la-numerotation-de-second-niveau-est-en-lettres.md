# BUG-049 numérotation de second niveau en chiffres romains

Même sans numéroter le niveau 1, dès que le niveau deux est numéroté il s'écrit sous forme de chiffres romains i, ii (ce qui est peu compréhensible si on veut avoir une grande lisibilité pour plus tard effectuer de la traçabilité).

## Historique

- statuts : ouvert_260322_() / 
- contexte : [les liste en markdown](https://www.markdownlang.com/fr/basic/lists.html) peuvent avoir plusieurs niveaux, mais comment garder ces niveaux au format numérique

## Criticité

- impact : fonctionnalité dégradée, manque de visibilité de la hiérarchie
- fréquence : moyenne (recours aux listes numérotes pour la traçabilité des expressions de besoins)
- detection : haute
- contournement : ne pas utiliser la numérotation en liste de niveau 2 (en niveau 1 la numéroation est en chiffre)

## Correction

- arbitrage : il serait bien d'avoir une compatibilité maximum avec le langage markdown (même si effectivmentle i, ii est pratiqué)
- correctif : voir s'il  existe une option dans la librairie externe
- changement : (on peut voir ci dessous i, ii, tant que incident non résolu)
    1. voir s'il y a une option de configuration dans l'outil tierce
    1. soit signaler l'incident à l'éditeur et attendre une montée de version corrective
    1. ou gestion par simple css en enlevant les chiffres romains

## Analyse

- cause racine : dépendance externe
