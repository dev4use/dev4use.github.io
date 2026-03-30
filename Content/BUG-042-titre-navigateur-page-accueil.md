## BUG-042 le titre de la derniere page listée en plan de site est le titre navigateur de la page d'accueil

- statuts : ferme_260315_() / ouvert_260315_()
- contexte : l'accueil est géré à part par une page txt qui est traitée par une fonction personnalisé
- événement : à l'arrivée sur site ou au retoiur à l'accueil par lien de menu, le titre de navigateur est celui du dernier post listé en plan de site
- impact : cosmétique
- fréquence : forte
- détection : moyenne, qui regarde le titre en url à pmart les moteurs de recherche ?
- contournement : aucun
- arbitrage : la page d'accueil donne l'impression première et est donc assez importante
- correctif : utiliser le titre de l'application déjà mis en fichier de configuration
- rex : non testé avec attention, pose la question des doublons de code entre 2 fonctions de generation de fichier
- cause racine : confiance
