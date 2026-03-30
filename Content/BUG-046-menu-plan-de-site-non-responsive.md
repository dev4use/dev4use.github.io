## BUG-046 le menu de plan de site est non responsive 

- statuts : ferme_260316_(fermé, pour l'instant ?) / ouvert_260316_() / 
- contexte : la catégorie est présente par préfixe du nom de fichier, donc si on transforme le path en label...
- événement : afficher le site sur un écran réduit fait se poursuivre la liste de catagorie 1 sur la catégorie 2 qui devient illisible
- impact : bloquant
- frequence : moyenne
- detection : moyenne, avoir un petit écran pour le détecter au plus vite
- contournement : aucun
- arbitrage : nuit à l’image de marque et rend inaccessible des posts
- correctif : FIX-022 / 
- changement : adapter la feuille de de style, déplacer la hauteur sur l'item de c haque liste (li)
- rex : non testé avec beaucoup de contenu
- cause racine : test
