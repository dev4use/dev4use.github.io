# EB-017 un plan de site plus restreint et plus approprié

Pour guider le lecteur dans un site qui prend de l'ampleur, en plan de site, présenter par défaut les posts liés à la rubrique.


## Propositions

- Statuts : enonce_20260411
- Solution : cibler les posts de la catégorie en cours
    - Parce que cela dépend du nombre de posts, laisser la décision à l'administrateur en présentant une gestion par configuration (pour l'instant, ne pas détecter automatiquement la quantité de posts et laisser le système décider : ou fixer le seuil en configuration).
    - Lorsque l'option est activée en configuration, seuls les posts de la catégorie sont affichés.
    - Sous les posts de la catégorie, un bouton "voir plus" permet d'afficher les posts des autres catégories.

## Arbitrages

- Importance : moyenne - le site va devenir de moins en moins ergonomique
- Urgence : basse - le positionnment du site actuel et de la version STANDARD peut excuser cette lacune ergonomique
- Difficulté : moyenne - alimenter deux listes (seulement la catégorie actuelle, seulement les autres catégories)

## Contrôles

- Assertions :
    - En cas de non activation de l'option, rien ne change (ou lorsque le seuil n'est pas atteint).
    - En cas d'activation de l'option, seuls les posts de la catégorie sont visibles.
    - En cas d'activation de l'option, un lien "en savoir plus" est visible.
    - En cas d'activation de l'option, au clic sur le lien "en savoir plus", toutes les autres catégories sont visibles avec leur post.
