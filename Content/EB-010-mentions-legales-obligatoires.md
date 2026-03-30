# EB-010 exposer les mentions légales

- Besoin : les sites pro ont besoin de mentions légales, quant au particulier ce n'est pas si clair. Mais dans le doute...
- Statuts : realise_20260321 / enonce_20260318
- Solution : 
    - présenter la page en footer
    - ajouter un footer
    - gérer la page en contenu normal dans le dossier de contenu
    - exclure cette page (et d'autres éventuelles du même type) grâce à un pattern, du type "fausse catégorie" FOOTER-
    - laisser le choix du nom de ce préfixe à exclure en configuration
- Importance : haute
- Urgence : haute
- Difficulté : moyenne - exclusion dans l'algo, css du footer
- Assertions : 
    - le fichier FOOTER est présent en page de referentiel
    - le fichier FOOTER est absent de la page plan de site
    - le lien vers le fichier FOOTER est visible en footer (test IHM)
    - le lien vers le fichier FOOTER affiche au clic la page concernée (test IHM)