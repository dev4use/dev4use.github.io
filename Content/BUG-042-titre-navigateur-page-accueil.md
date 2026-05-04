# BUG-042 en accueil, le titre navigateur est celui du dernier post de plan de site

 A l'arrivée sur site ou au retour à l'accueil par lien de menu, le titre de navigateur est celui du dernier post listé en plan de site.

## Historique

- statuts : ferme_260315_() / ouvert_260315_()
- contexte : l'accueil est géré à part par une page txt qui est traitée par une fonction personnalisée.

## Criticité

- impact : cosmétique
- fréquence : forte
- détection : moyenne, qui regarde le titre en url à part les moteurs de recherche ?
- contournement : aucun

## Correction

- arbitrage : la page d'accueil donne l'impression première et est donc assez importante
- correctif : utiliser le titre de l'application déjà mis en fichier de configuration

## Analyse

- rex : non testé avec attention, pose la question des doublons de code entre 2 fonctions de generation de fichier
- cause racine : confiance
