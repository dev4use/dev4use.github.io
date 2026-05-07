# BUG-048 barrer un texte en markdown

RESOLU: Barrer un texte en markdown ~~de la sorte~~ par des tildes ne fonctionne pas avec la libaririe externe utilisée.

## Historique

- statuts : ferme_260507_(ajout de la lib) / ouvert_260322_() 
- contexte : [un texte peut être barré en markdown](https://www.markdownlang.com/fr/extended/strikethrough.html) pour signifier une rature, une obsolescence, un repentir, et a une signification forte qui doit être gardée en html

## Criticité

- impact : fonctionnalité non délivrée, effet cosmétique
- fréquence : basse (pas tous les jours qu'on barre du texte et laisse ce texte dans un document, ~~sauf~~ dans des specs, solutions...)
- detection : moyenne (tomber sur le cas) mais facile (se voit à l'oeil nu)
- contournement : ne pas utiliser le tilde de suppression

## Correction

- arbitrage : il serait bien d'avoir une compatibilité maximum avec le langage markdown
- correctif : voir s'il ne faut pas une extension supplémentaire dans la librairie externe
- changement : 
    - [X] soit ajouter l'option de l'extension : installer pymdown-extensions et appeler extensions=['pymdownx.tilde']
    - [ ] soit signaler l'incident à l'éditeur et attendre une montée de version corrective

## Analyse

- cause racine : dépendance externe
