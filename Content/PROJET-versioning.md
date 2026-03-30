# Versionning logiciel

Pour maintenir le cycle de vie de plusieurs versions d'un même produit en parallèle, il faut être organisé.

## Gestionnaire de code source

Ces niveaux de produit peuvent se matérialiser par des préfixes de tags de version :

 - ST- pour STANDRD
 - PR- pour PREMIUM
 - OP- pour OPTIMUM

 Ces versions appliqueront le système [SEM](https://semver.org/lang/fr/) : MAJEURE.MINEURE.CORRECTIF.
 Le préfixe cité plus haut sera apposé.   
 A noter que la recommandation est de ne pas gérer les préfixes de zéro, soit 9 vers 10 et non 09 vers 10 (ce qui peut gêner le classement alphabétique).  
 Une fois approprié, ce système de notation se traduit par :

 1. version complète et cohérente pour son niveau d'ambition,
 1. nouveauté fonctionnelle,
 1. correctif.

## Structure de fichiers

Chaque version du produit pourra être maintenue conjointement par un système de fichiers du type :

- Code :
    - workflow : squelette de l'application, ensemble ordonné des traitements, tel un plan batch.
    - common : code source partagé par toutes les versions
    - interface : méthodes utilisées par tous, en format plus ou moins dégradé jusqu'à être à vide.
    - standard : fonctions propres à cette version
    - premium : fonctions propres à cette version
    - optimum : fonctions propres à cette version
