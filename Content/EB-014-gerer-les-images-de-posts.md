# EB-014 gérer les images de post

Pour illustrer leurs propos, les post comportent des images.

## Propositions

- Statuts : enonce_20260322
- Solution : gérer les images liées aux posts
    - En dossier "Content" (ou Content/Images), les images strictement nommées comme leur post d'appartenance et numérotées en préfixe de type -1... seront identifiées comme liées au post par le système.
    - Les images seront affichées dans le rendu html du post à l'emplacement où elles étaient insérées en markdown.
    - La première image (selon la numérotation) sera gérée en vignette de post (pour la page listing de posts dans une catégorie).

## Arbitrages

- Importance : haute - un site sans image est peu attractif
- Urgence : basse - le positionnement du site actuel et de la version STANDARD peut expliquer uen absence d'image
- Difficulté : moyenne - script d'optimisation et réduction d'image (pour la vignette)

## Contrôles

- Assertions :
    - Toutes les images d'un post sont présentes dans le post.
    - En page catégorie, la vignette est l'image 1.
    - En page catégorie, la vignette est de taille réduite comparée à l'originale (si l'originale était supérieure à la taille de l'encart attendu).
