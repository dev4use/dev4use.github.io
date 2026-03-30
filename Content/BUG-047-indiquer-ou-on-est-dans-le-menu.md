## BUG-047 visualiser la page en cours dans le menu

- statuts : ouvert_260316_() / ferme_260318_(peu propre et consommateur de ressources)
- contexte : le menu est immuable, la page en cours n'est pas indiquée, contrairement aux standards du web
- événement : dans le menu, on peut recliquer sur la page où on est sans le savoir, car notre position n'est pas indiquée
- impact : ergonomie
- frequence : élevée
- detection : moyenne, avoir u n petit écran pour le détecter au plus vite
- contournement : le nom de l'url est explicite pour indiquer notre position
- arbitrage : nuit à l’image de marque et rend inaccessible des posts
- correctif : FIX-023 / 
- changement : 
    - adapter la feuille de style
    - appliquer active à la page en cours
    - se refuser la facilité d'une solution js, js en dernier recours, philosophie de l'applicatif
    - un peu quick and dirty : benchmarker un jour avec remplacement par sub ou autre 
- rex : pas vu, menu commun généré avant la boucle de post à déplacer dans la boucle (mais redondance en consommation)
- cause racine : test
