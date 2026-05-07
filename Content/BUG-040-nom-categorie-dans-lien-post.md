# BUG-040 le nom de la catégorie est répété en libellé de chaque post 

RESOLU: La liste horizontale des posts met en évidence la répétition du nom de la catégorie.

## Historique

- statuts : ferme_260315_(fermé, plus simple que prévu) / ouvert_260314_() / 
- contexte : la catégorie est présente par préfixe du nom de fichier, donc si on transforme le path en label...


## Criticité

- impact : cosmétique
- frequence : élevée, dans le plan de site facilement visible
- detection : facile, visible dès l’accueil
- contournement : aucun
- arbitrage : nuit à l’image de marque

## Correction

- correctif : FIX-020 / retirer la catégorie du label lors de la récupération en liste
- changement : ajouter la variable categorie et déplacer dans l'algo après l'interception de la catégorie

## Analyse

- rex : manque de bon sens dans le contrôle, aurait pu être vu avant
- cause racine : confiance
