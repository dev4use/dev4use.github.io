# EB-013 exposer des pages de listing catégorie

Disposer de pages par catégorie, le problème se pose(ra) avec un nombre élevé de posts par catégorie rendant l'affichage en menu de header pénible aux yeux.

## Propositions

- Statuts : lot_01_20260502 / enonce_20260322 /
- Solution : se conformer aux standards du marché en offrant des pages catégorie
    - lot_01 :  en menu de header, avoir un lien sur la catégorie amenant à la page catégorie
    - en menu header (lié à l'EB-012 de gestion des dates), afficher juste les unièmes posts les plus récents (nombre gérable en configuration)
    - lot_01 : présenter des pages catégories
    - lot_01 : en configuration, ajouter une description possible de chaque catégorie (un peu intrusif, limite pour la philosophie de la version STANDARD, gérer un contenu éditorial propre au site) / cette configuration pourra servir à choisir le template type du post dans une version plus évoluée
    - réaliser une pagination des posts (la priorité de la fonctionnalité sera liée au volume de post)
    - lié à la question du volume, afficher devant la catégorie le nombre présent (quel service réellement rendu ?)

## Arbitrages

- Difficulté : moyenne - rajouter des fonctions d'affichage dans la version STANDARD sans template est un peu lourd

## Contrôles

- Assertions :
    - Le nom de la catégorie du header comporte un lien vers la page de sa catégorie.
    - La page de la catégorie affiche une description lorsque la description est présente en configuration.
    - La page de la catégorie n'affiche aucune description lorsque la description est absente en configuration.
    - Proche du nom de catégorie en header, figure le nombre de posts qui correspond au nombre de posts publiés.
    - Proche du nom de catégorie en page catégorie, figure le nombre de posts qui correspond au nombre de posts publiés.
    - Une catégorie sans posts, présente en page de configuration, avec ou non sa description, est absente en menu et absente en page catégorie. 
