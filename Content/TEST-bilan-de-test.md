# Bilan de test

Si vous pensez au PV de recette, en tant que référentiel de haut niveau, l'ISTQB n'entre pas dans ce niveau de détail et ne cite pas un tel document.   
Il existe plusieurs niveaux de bilan de tests :

- par niveau de test,  
- par application,  
- par application et niveau de test,  
- sur une excécution,  
- sur une campagne,   
- sur une release,    
- sur un projet.  

Difficile de savoir de quoi on parle.  
Ce qui manque peut-être ajourd'hui, mais peut-être pas demain dans le référentiel ISTQB au tournant Agile(A) affirmé, c'est l'angle rétrospective.  

## Contexte de la mission Marss

En testant l'application <a href="https://github.com/dev4use/marss" class="trademark">Marss</a>, certains éléments sont ressortis :

### Testabilité :  

En version ST-01,   

- Le fichier de configuration initialisé et aujourd'hui partagé en globale est le point d'accès principal et redondant en test. Vivement le passage en classe où cette phase d'init sera plus assumée.   
- Certaines balises html ont été retravaillées pour être plus faciles à atteindre en tests, mais aussi pour facilier leur gestion et robustesse en développement css.  

Analyse :

- En assumant les deux rôles développeur et testeur, il devient visible en quoi la collaboration développeur/testeur peut être bénéfique pour les deux parties. 

### Effort de test :

En version ST-01,   

- Viser une couverture de code à 100 % par les tests   
- et utiliser la conception de test BDD au format Gherkin, qui plus est souvent au niveau unitaire,   

semble parfois contre-productif ou absurde.

Analyse :

- Pratique pour l'instant assumée au titre d'une démonstration de mise en oeuvre.


*Notes :*    
A/ L'ISTQB a pris comme prétexte le tournant Agile pour vulgariser et simplifier au point de vider certaines notions de leur substance ou de faire disparaître ces notions.  
