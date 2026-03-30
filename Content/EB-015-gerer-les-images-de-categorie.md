# EB-014 gérer les images de catégorie

- Besoin : pour illustrer leurs propos, les post comportent des images
- Statuts : enonce_20260322
- Solution : gérer les images liées aux posts
    - En dossier "Content" (ou Content/Images), les images strictement nommées comme leur catégorie d'appartenance (voir préfixe de post et fichier de configuration) seront identifiées comme liées à la cétagorie par le système.
    - La dite image sera gérée en vignette de post (pour la page listing de posts dans une catégorie).
    - Une seule image sera affichée et autorisée par catégorie (règle d'attribution sans importance en cas d'images multiples pour une même catégorie).    
- Importance : haute - un site sans image est peu attractif
- Urgence : basse - le positionnment du site actuel et de la version STANDARD peut expliquer une absence d'image
- Difficulté : moyenne - script d'optimisation et réduction d'image (pour la vignette)
- Assertions :
    - En page catégorie, la vignette de catégorie est l'image de catégorie.
    - En page catégorie, la vignette est de taille réduite comparée à l'originale (si l'originale était supérieure à la taille de l'encart attendu).
    - En l'bsence d'image pour une catégorie, aucune imge n'est affichée et aucune erreur liée n'apparait à l'affichage.
    - En présence de plusieurs images pour une catégorie, le script de génération provoque un vartissement explicite mais continue son traitement.
