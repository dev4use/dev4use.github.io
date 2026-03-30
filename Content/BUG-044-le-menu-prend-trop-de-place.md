## BUG-044 le menu plan de site peut prendre trop de place

- statuts : ferme_ (20260320) / ouvert_260315_()
- contexte : le menu reste tout le temps déplié
- événement : sur un post, le menu déplié à la verticale va très vite prendre tout l'écran
- impact : majeur (captitalise l'attention)
- fréquence : forte, sur chaque page
- détection : forte, cela se voit dès qu'on clique pour faire apparaître le menu
- contournement : l'utilisateur n'a qu'à pas cliquer, il n'est dérangé que temporairement et "volontairement"
- arbitrage : c'est aussi une question d'image de marque que d'afficher un contenu accessible assez vaste
- correctif : AM-001 aligner le menu à l'horizontale, avec séparateur et avec moins de hauteur, tout cela en CSS
- rex : simplicité, épure parfois trop importante
- cause racine : ergonomie
