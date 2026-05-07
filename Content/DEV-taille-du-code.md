# Maîtriser la taille du code

Une application est composée de code source, si si je vous le dis. Et même en No Code (LOL). Le code source est donc un facteur à prendre en considération... qualité et quantité.

## L'influence de la taille du code

Plus il y a de code, plus il y a de risques de défauts. Ce principe est tenu pour axiome (pas par moi, par la communauté logicielle).  

Limiter la croissance du code, du moins mesurer et maîtriser l'accroissement du code source est donc une décision censée.   

Mais il faut contrebalancer cette intention par **le principe de précaution**. Dès qu'une métrique est mise en place, sitôt comprise, la métrique peut être faussée lorsque les comportements humains changent en vue d'obtenir de meilleurs scores. 

Pour que le opérateurs restent focalisés sur leur travail habituel, un focus sur d'autres facettes de la valeur produite par leur travail peut être effectué.

Dans un contexte Agile, si on se réfère ([une fois de plus](PROJET-us-projet-jetable.md#un-gachis-volontaire)) au 
[manifeste Agile](https://manifesteagile.fr/) :

> "Porter continuellement attention à l’excellence technique et à la qualité de la conception renforce l’agilité."

Mais il ne faut pas se méprendre sur la valeur de l'excellence. Ce pourrait être [un autre point polémique](PROJET-us-projet-jetable.md).  
L'excellence du code est un juste équilibre entre plusieurs facteurs :

- la performance du code ou toute autre considération qui entre en ligne de compte dans l'application,   
- la lisibilité du code,  
- la maintenabilité du code.

Il faut **un juste niveau de qualité**. 

> Une excellence/optimisation extrême du code rendrait le code incompréhensible, inexploitable et inmaintenable par tout autre membre de l'équipe que son concepteur expert. 

Or, en Agile version utopique, les membres de l'équipe ont des postes interchangeables.   

## Le code interne

L'objectif, surtout avec la version STANDARD est de rester modéré en taille d'application et nombre de lignes de code.   
Pour information, cette taille est mesurée par pygount.   
L'objectif est de vérifier qu'il n'y a pas un effet d'emballement dans le temps.   
Pourrait exister une courbe de croissance de ce type :


| numero de version | valeur acquise | taille atteinte | valeur du code |
| ---- | ---- | ---- | ---- |
| 1 | 30 | 300 | 10 |
| 2 | 33 | 300 | 9 |



Vous allez peut-être me dire que vous ne savez pas mesurer la valeur (quand bien-même vous seriez en méthode Agile) ? Touvez/inventez un autre élément de mesure.

## Le code externe

L'application utilise des librariries tierces.  
Ces librariries tierces contiennent des lignes de code qui viennent s'ajouter aux premières.  
Cette seconde taille est le plus souvent masquée et ignorée.   
L'objectif est de mettre en évidence cette seconde taille. Cela permet de mesurer la taille "réelle" totale de l'application.     

