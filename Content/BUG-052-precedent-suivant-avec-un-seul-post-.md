# BUG-052 erreur fatale pour lien suivant precedent avec un seul post

RESOLU: La génération du site échoue à l'étape d'affichage du menu précédent suivant pour un post seul dans sa rubrique.

## Historique

- statuts : ferme_260507_() /ouvert_260507_()
- contexte : les éléments url et label des liens précédent et suivant ne sont pas générés et ne peuvent donc être affichés

## Criticité

- impact : bloquant
- fréquence : haute, si publication progressive avec 1 seul post au départ dans 1 rubrique nouvelle
- detection : facile, la génération du site échoue en console à cette étape
- contournement : aucun

## Correction

- arbitrage : à corriger puisque bloquant
- correctif : oui
- changement :
    - en fonction d'affichage, test d'existence des clés url et label dans les dictionnaires precedent et suivant
    - ajout de tests automatiques pour aller au bout et gérer ces cas pourtant connus aussi en étape d'affichage

## Analyse

- cause racine : erreur humaine, dissociation des responsabilités. Cas géré en génération de variables et en couverture de tests de ces variables, mais oublié en affichage HTML de ces variables.
