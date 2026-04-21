# BUG-041 un hyperlien en extension md n’est pas transformé en html

Au clic sur le lien en extension .md, on aboutit à une erreur 404.

## Historique

- statuts : ferme_260316_(fixé assez légèrement, sûrement peu robuste) / ouvert_260314_()
- contexte : puisque le md est traduit en html, on s’attend à ce que la transformation soit complète. Il s’agit d’une librairie externe.

## Criticité

- impact : bloquant ( l’action ne peut aboutir)
- fréquence : faible, les liens entre fichiers ne sont pas constants par contenu
- détection : moyenne, l’utilisateur doit cliquer sur le lien pour savoir qu’il est brisé
- contournement : l’utilisateur saisit par anticipation l’extension .html dans son fichier .md

## Correction

- arbitrage : la version de l’application veut imposer le moins de contraintes possibles lors de la création du .md, donc le correctif est nécessaire
- correctif : détecter la présence d’un hyperlien (au plus tôt en md et non en html ?) en .md et changer l’extension en .html

## Analyse

- rex : trop grande confiance accordée à une dépendance
- cause racine : confiance