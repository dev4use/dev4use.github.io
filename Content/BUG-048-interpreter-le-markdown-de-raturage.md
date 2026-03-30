## BUG-048 barrer un texte en markdown

- statuts : ouvert_260322_() / 
- contexte : [un texte peut être barré en markdown](https://www.markdownlang.com/fr/extended/strikethrough.html) pour signifier une rature, une obsolescence, un repentir, et a une signification forte qui doit être gardée en html
- événement : barrer un texte en markdown ~~de la sorte~~ par des tildes ne fonctionne pas avec la libaririe externe utilisée
- impact : fonctionnalité non délivrée, effet cosmétique
- fréquence : basse (pas tous les jours qu'on barre du texte et laisse ce texte dans un document, sauf dans des specs, solutions...)
- detection : moyenne (tomber sur le cas) mais facile (se voit à l'oeil nu)
- contournement : ne pas utiliser le tilde de suppression
- arbitrage : il serait bien d'avoir une compatibilité maximum avec le langage markdown
- correctif : voir s'il ne faut pas une extension supplémentaire dans la librairie externe
- changement : 
    - soit ajouter l'option de l'extension
    - soit signaler l'incident à l'éditeur et attendre une montée de version corrective
- cause racine : dépendance externe
