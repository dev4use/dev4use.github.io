# Dette technique du code source

Ce n'est pas vraiment ce qui s'appelle terminer en beauté. En aboutissement fonctionnel de version STANDARD, je prends la mesure de la dette technique.

![dette technique](../Media/dette-technique.jpg "dette technique")

## Une dette assumée

Si certains points sont assumés et dès le départ, je pense à des partis pris techniques tels que :

- codage précédural en fonctions sans classes,
- absence de recours à des templates de présentation IHM,

d'autres points relèvent plus de fautes de conception.

## Une faute de conception

Là encore, pour être sincère, ces problèmes de conception ne sont pas totalement une suprise.   
J'ai pris le parti de coder à mesure, sans forcément de plan complet précis, juste une cinématique générale issue de la logique.  
J'assume cette position dans un autre article : adaptabilité et maintenabilité (un mal pour un bien).   

## Une dette involontaire

Mais en ayant recours à des subterfuges que je m'interdisais, je comprends que je subis la situation.

Je me vois dans l'obligation, pour terminer cette version en l'état, d'en arriver à certains expédients.  
Expédient, le mot est juste.   
**Pour expédier/délivrer ce produit sans tout changer au dernier moment**, je dois recourir aux procédés suivants que je m'interdisais :

- fonction de niveau intégration : une fonction qui en appelle d'autres,
- duplication de code (pour aller plus vite sur l'instant),
- helper purement technique,
- perte de traçabilité et de responsabilité unique (ou presque) d'une fonction.

Je fais référence à des éléments de code clairement identifiés (version/release : ST-2... , tags : ST-2...) :

- ```afficherPostsDeCategorie``` : fonctions incluses, sinon il aurait fallu modifier le fichier référentiel,
- ```extraitDeMarkdown et nombreDeMots``` : duplication de code en l'absence de fonction du type retirer_blalises_markdown,
- ```helper_fichierCorrespondance``` : helper pour relier deux référentiels incompatibles entre eux (plutôt que de refactorer de suite et unifier),
- ```ajouterEtTransformerEnHtml``` : cache des fonctionnalités que je ne retrouvais pas, et pour cause :
    - affichage des menus de page et de site...

Je peux également ajouter le besoin de distinguer explicitement les types de fonction, comme : 

- les fonctions purement d'affichage (hélas avec cette absence volontaire de template),
- les fonctions de traitement du flux de données,
- les fonctions techniques de transformation et d'enrichissement,
- etc.

Adopter une norme de nommage par préfixe par exemple.

## Une prise de conscience

J'ai néanmoins conscience de la situation.   
J'assume mes actes réalisés par pragmatisme : engranger de la dette technique à la dernière étape pour boucler le dossier.   
Ce sera juste pour mieux réouvrir le dossier dans une version ultérieure.

## Une prise de risque limitée

Il s'agit d'adopter une posture pragmatique qui serait également économique en milieu professionnel et en respectant des conditions financières.     

Pour cette raison, un bug identifié est laissé : [absence d'infos dates et temps de lecture sur un post seul dans une rubrique](BUG-045-posts-sans-dates.md).  
L'incident est limité à un contexte particulier et rare et avec peu d'impact, donc avec une criticité (et donc un risque) faible.

Les prédicateurs ou moralisateurs qui savent tout pondraient ces sentences de leur extraordinaire derrière :  

- Tout bien faire du premier coup n'est pas réaliste. 
- Un perfectionnisme excessif aboutit à l'immobilisme. 
- Ce n'est jamais totalement fini. On trouve toujours à redire, à retrancher ou à ajouter...

