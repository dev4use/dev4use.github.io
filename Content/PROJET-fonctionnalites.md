# Liste des fonctionnalités

Une application offre un ensemble de fonctionnalités.
Lorsqu'il existe une pluralité de versions, ces versions peuvent décliner des mêmes fonctionnalités dans un niveau de services différent.

## Déclinaison de l'offre

A noter une perméabilité descendante ou rétrocompatibilité des versions.
Une version supérieure doit être capable de réaliser les opérations d'une version inférieure. Cette possibilité doit rester offerte à l'utilisateur.
 > Principe du : qui peut le plus peut le moins.

Déclinaison de l'offre visible à travers les sous dossiers :

- WebServer : serveur 
    - ST : python http (dossier inexistant dans cette offre),
    - PR : gunicorn,
    - OP : nginx https et N backend pour réaliser un hébergement plus conforme aux standards.
- Content : contenu
    - ST : à déposer,
    - PR : récupéré d'autres dossiers
    - OP : récupéré du cloud.
- Themes : templates
    - ST : uniques pour un seul design,
    - PR : réparties dans un thème parmi d'autres
    - OP : téléchargeables et installables comme un système de plugin.
