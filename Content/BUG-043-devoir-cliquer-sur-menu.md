## BUG-043 chaque page est une impasse, pas de lien direct vers une autre page

- statuts : ferme_260315_() / ouvert_260315_()
- contexte : la version première du standard se présente comme une seule page, avec une économie d'informations autres
- événement : il faut cliquer sur "menu site" pour accéder aux liens menant vers els autres pages du site
- impact : minime (juste un clic à faire)
- fréquence : forte, sur chaque page
- détection : forte, cela se voit qu'on arrive sur une impasse
- contournement : l'utilisateur n'a qu'à réaliser un clic de plus
- arbitrage : c'est aussi une question d'image de marque que d'afficher un contenu accessible assez vaste
- correctif : AM-002 pouvoir afficher le menu d'emblée, ajouter une option de configuration pour choisir le menu ou aucun, et gérer la condition dans le code pour activer le menu sous forme de checked
- rex : simplicité, épure parfois trop importante
- cause racine : ergonomie