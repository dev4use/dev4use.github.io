# EB-016 accélérer le temps de chargement des pages du site par la mninification

- Besoin : pour accélérer le temps de chargement des pages du site, compresser les éléments
- Statuts : enonce_20260322
- Solution : optimiser les contenus
    1. Compresser le css, ajouter "minify" en suffixe, et lier le fichier au html.
    2. Compresser le html généré
- Importance : moyenne - les temps d'affichage peuvent (vite ?) devenir problématiques (un comble pour un site statique)
- Urgence : basse - dédié à une version OPTIMUM de la solution
- Difficulté : moyenne - des scripts python existent (sont-ils encore maintenus ?)
- Assertions :
    1. Mesurer la taille du fichier CSS avant/après.
    2. Mesurer la taille du fichier HTML avan/apres.
    3. Vérifier en html final que le fichier css lié est bien le "minify"
