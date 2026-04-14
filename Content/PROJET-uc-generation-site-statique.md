# Cas d'utilisation textuel : génération du site statique

Application présentée en cas d'utilisation textuel, tel que prôné par Alistair Cockburn.

## Contexte :

Acteur principal : Le système  
Acteur(s) secondair(es) : Le développeur(A)  

Portée : site statique en local  
Contexte d'utilisation : Le développeur veut générer un site statique.  
Préconditions :  

- Repo du code source récupéré, 
- dossier de contenu disponible,
- fichier de configuration personnalisé, 
- développeur connecté à la console.  

Déclencheur : Le développeur lance la commande de génération du site.  
Fréquence : à chaque modification de contenu markdown que souhaite visualiser ou embarquer le dévelopeur, le système recrée la totalité du site statique.  
Garanties en cas de succès : Le développeur navigue en local sur le site statique.  
Garanties minimales (en cas d'échec) : Le développeur voit le programme s'arrêter sur un message d'erreur explicatif.   

## Scenario  nominal :

1. Le développeur lance la commande de génération de site statique.
1. Le système récupère la configuration et la liste les fichiers markdowns.
1. Le système crée un référentiel de pages complet enrichi.
1. Le système prépare l'affichage html des éléments de menu.  
1. Le système capture le contenu de chaque markdown, l'enrichit et le transforme en html.
1. Le système assemble l'ensemble des éléments html en un seul contenu html.
1. Le système crée chaque fichier html dans le dossier du site statique et y déplace les éléments de style.
1. Le système lance un serveur de debug et ouvre le site statique dans le navigateur.
1. Le développeur visualise son contenu et peut naviguer dans le site.


## Variantes : 

4.A  Si le système ne trouve aucune page pour alimenter les liens de pied de page,

 - les liens de pied de page ne sont pas retournés,
 - aucune erreur n'est signalée au développeur,
 - le traitement suit son cours.

## Extensions :

*A  Le système indique en console les étapes et les éventuelles erreurs.  

2.A Si le chemin du répertoire de contenu markdown n'est pas renseigné,

  -  une erreur signale l'incident
  - et le traitement s'arrête.  


2.B  Si le chemin du répertoire de contenu markdown n'est pas trouvé sur l'espace disque,  

  -  une erreur signale l'incident
  - et le traitement s'arrête.  


2.C Si le répertoire renseigné et trouvé est sans contenu de type markdown,

  - une erreur signale l'incident
  - et le traitement s'arrête.


*Notes :*  
- A/ L'utilisateur endosse le rôle de développeur de par sa capacité à récupérer un repo git, à modifier une configuration, et à lancer des lignes de commande en console de type linux.  