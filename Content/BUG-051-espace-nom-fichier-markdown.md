# BUG-051 oubli d'espace en nom de fichier markdown

En regardant attentivement les urls, il m'arrive de voir des pourcentages liés aux espaces/vides/blancs en nom de fichier.

## Historique

- statuts : ouvert_260328_()
- contexte : erreur humaine finalement assez fréquente, je ne vois pas que j'ai écrit des noms de fichiers markdown avec espace

## Criticité

- impact : pratiquement invisible
- fréquence : moyenne
- detection : facile, en barre de navigation
- contournement : aucun

## Correction

- arbitrage : même si c'est une erreur humaine, anticiper et se prémunir de cette erreur pour rendre service à l'utilisateur et futur lecteur
- correctif : oui
- changement :
    - en nom de fichier html, remplacer un espace vide (hérité du fichier markddown) par un trait
    - s'autoriser aussi à réécrire le fichier markdown source se trouvant dans le répertoire de contenu ? Non, ne pas être intrusif
    - notifier l'erreur en console

## Analyse

- cause racine : erreur humaine
