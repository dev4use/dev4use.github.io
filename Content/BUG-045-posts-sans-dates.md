## BUG-045 les posts n'ont pas de date

- statuts : ouvert_260315_()
- contexte : contrairement aux blogs classiques, les billets sont sans date
- événement : visualiser un billet seul et noter l'absence de date
- impact : mineur (très peu d'intérêt)
- fréquence : forte, sur chaque page
- détection : moyenne, encore faut-il y faire attention
- contournement : aucun, ou on a reperé que le billet n'était pas présent avant
- arbitrage : ce n'est pas une anomalie mais la question est légitime, un repère temporel est utile pour indiquer le degré de fraîcheur de l'information
- correctif : EB-012 dans cette version, gérer les dates de création et modification des fichiers md et les véhiculer en référentiel pour affichage, et par configuration activer ou non cet affichage voir cet ordre de tri
- rex : simplicité, épure parfois trop importante
- cause racine : ergonomie