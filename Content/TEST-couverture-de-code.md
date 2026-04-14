# La couverture de code par les tests

Pratique assez controversée, la couverture de code par les tests est quantitative mais peut néanmoins servir de garde fou.  

## Instaurer une fausse confiance

Dans <a href="https://github.com/dev4use/marss" class="trademark">Marss</a>, j'ai recours à la couverture de code, et à une couverture à 100 % pour [une livraison officielle majeure.](PROJET-versions-editeur.md#approches-qualite)  

Il s'agit de rassurer l'éventuel utilisateur.   
Mais si je veux au contraire inquiéter cet utilisateur (qui le veut, qui le doit parfois si nécessaire ?), je peux aussi le faire.   

Le test exécute l'ensemble du code et des branches (dans ma configuration de pytest --cov et coverage). Oui, le test "exécute".   
Si j'enlève la totalité des assertions, le test continue de s'exécuter et la couverture se maintient à 100 %.  

1. Rien sur l'existence des tests à proprement parler ou des assertions.  
1. Rien sur les éléments contrôles par les assertions et la pertinence de ces éléments.  

> Autrement dit, un testeur peut tester "à côté", tout en testant/exécutant "tout"

Cela, il faut le dire, quelque part comme dans [la politique de test](TEST-politique-de-test.md). Il faut le dire afin de :  

- clarifier la situation,
- ne pas insuffler un niveau de confiance illégitime dans la qualité de l'application et des tests,
- ne pas réaliser une **campagne de désinformation**.  

## Un moyen de travailler

Cela ne veut pas dire que connaître la couverture de code par les tests est inutile.  
Admettons que moi développeur/testeur je veux bien faire et ai pour objectif de tout tester, du moins ce qui me semble principal.  
Je peux contrôler si je n'ai rien oublié en faisant une couverture de code. Le rapport me montre que, tiens, j'ai oublié un petit point.  

*Arbitrage à faire :*  

Point trivial, à ne pas tester car la rentabilité n'y serait pas :   
l'exclure du rapport de couverture par la pattern adéquat, tel que ```# pragma: no cover``` par exemple.   

Point important au contraire et nécessitant un investissement pour le couvrir :  
soit on l'ajoute à un test existant où il est cohérent et n'ajoute que peu d'asserts,   
soit on crée un test dédié pour mieux le suivre ou parce qu'il nécessite un nombre d'assert assez conséquent.

## Un outil de précision

Et si mes assertions vérifient réellement des points importants vis-à-vis de mon algorithme, de mon processus métier ou des points importants pour mes parties prenantes,  

> je teste "juste", juste là où il faut, en vérifiant juste ce qu'il faut.
