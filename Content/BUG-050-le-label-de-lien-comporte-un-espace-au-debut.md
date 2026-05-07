# BUG-050 le label de lien vers post débute par un espace

RESOLU: La création du référentiel html détecte les catégories, mais ce faisant, laisse un blanc en remplacement dans le label.

## Historique

- statuts : ferme_260325_() / ouvert_260325_()
- contexte : étape par étape, les données sont transformées, mais pas forcément vérifiées en pas à pas

## Criticité

- impact : pratiquement invisible
- fréquence : haute
- detection : difficile, voir le code source
- contournement : inutile, qui s'en rend compte ?

## Correction

- arbitrage : détecté par le test et corrigé aussitôt (typiquement un incident non communiqué qui passe en action de debug)
- correctif : oui
- changement :
    - ajouter un .strip() au label

## Analyse

- cause racine : ni test automatique ni code source scruté à la loupe
