# BUG-043 chaque page est une impasse, pas de lien direct vers une autre page

Il faut cliquer sur "menu site" pour accéder aux liens menant vers les autres pages du site.

## Historique

- statuts : ferme_260315_() / ouvert_260315_()
- contexte : la version première du standard se présente comme une seule page, avec une économie d'informations autres

## Criticité

- impact : minime (juste un clic à faire)
- fréquence : forte, sur chaque page
- détection : forte, cela se voit qu'on arrive sur une impasse
- contournement : l'utilisateur n'a qu'à réaliser un clic de plus

## Correction

- arbitrage : c'est aussi une question d'image de marque que d'afficher un contenu accessible assez vaste
- correctif : AM-002 pouvoir afficher le menu d'emblée, ajouter une option de configuration pour choisir le menu ou aucun, et gérer la condition dans le code pour activer le menu sous forme de checked

## Analyse

- rex : simplicité, épure parfois trop importante
- cause racine : ergonomie