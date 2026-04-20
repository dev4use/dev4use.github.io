# EB-011 remonter en haut de page

En cas de contenu important dépassant N fois la taille d'écran, remonter "facilement" en haut de page.

## Propositions

- Statuts : enonce_20260318
- Solution : élément visuel  en css de position fixe en bas de page dans une gouttière (espace vertical libre tout le long) à côté du contenu

## Arbitrages

- Importance : basse - contournement du raccourci clavier de remontée en haut de page
- Urgence : basse
- Difficulté : moyenne - effet de bord en responsive ?

## Contrôles

- Assertions :
    - le lien est présent en bas de page (test IHM)
    - au clic sur le lien présent, le lien amène en haut de page (test IHM)
