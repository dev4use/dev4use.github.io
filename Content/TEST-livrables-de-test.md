# Livrables de test

J'hésitais sur le terme :

- artefact - trop savant - ,
- [testware ISTQB](https://glossary.istqb.org/fr_FR/search?term=testware&exact_matches_first=true) - encore plus savant - ,
- documentation - prêtant à confusion - .  

Finalement, le terme de "livrable" pour tous les éléments produits par **le processus de test** semble plus approprié.   
Pris au pied de la lettre, ce terme signifie : 

> (dé)livrable produit par le test.  

## Contexte de la mission Marss

Dans le contexte projet <a href="https://github.com/dev4use/marss" class="trademark">Marss</a>, je livre l'ensemble des éléments de test :

- les outils de test (requirements.txt),
- les scripts de test automatique et leurs jeux de donnés,
- les rapports de tests automatique,
- les compte-rendus qualité (convention de nommage, couverture de code, quantité de code),  
- les choix stratégiques liés aux tests.  

## Contexte élargi

Le terme retenu, livrable, peut avoir plusieures connotations.  


### Livrable exploitable

Bien-sûr, tout n'est pas facilement montrable, exploitable, mais
> tout devrait être (dé)livrable à qui le réclame et est capable d'en tirer des enseignements.  

Le test est une activité basée sur la communication et la transparence. Tout document produit devrait donc pouvoir être accessible.
Il n'y a guère de question à se poser (  

- sinon sur la politique de sauvegarde et de stockage des données,
- sinon sur la durée de rétention des rapports et logs automatiques de tests....

).

### Livrable officiel

Seul un sous ensemble de tous les éléments produits par **l'activité de test** aura peut-être "le statut officiel de livrable" dans votre organisation.
Peu importe pour notre propos.

### Livrable exploité

Ce qui importe le plus, c'est l'utilité du livrable. A quoi bon produire le livrable si son utilité est nulle ou limitée ?

Je peux citer ici :

- une stratégie de test ou une approche de test ni suivie ni enrichie durant le test,  
- une communication de rapport de tests de régression qui comporte en évidence l'ensemble des tests (dont une majorité écrasante de tests OK), au lieu de ne communiquer que sur les tests NOK (tout en donnant un accès complémentaire à l'ensemble des autres tests).  

> Ce que vous faîtes est-il utile et donc utilisé ?

Parfois la réponse peut venir d'en haut : c'est demandé, imposé, contractuel. Vous réalisez une activité de conformité légale, point barre, circulez il n'y a à voir. Ce document est incompréhensible et ne sera lu qu'une fois et archivé ensuite.
Dommage si vous n'avez pas réussi à produire un deux en un qui aurait pu servir de fil rouge au processus de test. Mais tant pis, passez à autre chose.

## Liste des livrables

Listons les élements dans l'ordre pseudo chronologique de la cinématique de notre processus (processus forcément plus complexe avec imbrications et allers retours entre différentes phases).

- [politique de test](TEST-politique-de-test.md)
- ...
- [bilan de test](TEST-bilan-de-test.md)
