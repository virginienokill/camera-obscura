# Les soufflets

Pour effectuer la mise au point et lorsque l'on change de focale, il faut changer la distance entre l'écran et l'optique.
Or, quelque soit la position de l'optique par rapport à l'écran, il faut que la chambre reste hermetique à la lumière.

Pour concilier étancheité du dispositif et possibilité varier la position relative des deux parties,
la solution traditionnellement utilisée pour les chambres noires photographiques (mais aussi pour les accordéons et les autobus articulés) est celle du soufflet.

Bien que le choix du soufflet vienne apporter une solution très satisfaisante au problème décrit ci-dessus, il apporte aussi son lot de problèmes :
- Le patron d'un soufflet est difficile à dessiner.
- Le choix des materiaux est délicat (robustesse, souplesse, étanchéité, couleur)
- La construction d'un soufflet est chronophage.

## Dessiner un soufflet

On s'interesse ici à la construction de soufflets "coniques" et "rectangulaires".

### Préparation

Choix à faire avant de commencer :

- taille du grand cadre
- taille du petit cadre (côté objectif)
- largeur des plis
- nombre de plis
- La manière dont le soufflet est collé au grand cadre et au petit cadre.

Pour la largeur des plis on choisi en général 100mm ou 50mm. Puisque le soufflet est conique les plis mesureront une fois sur deux un peu plus et une fois sur deux un peu moins que la valeur choisie. Cette valeur est néamoins très importante pour dessiner le soufflet.

Le nombre de pli determinera la longueur du soufflet minimum et maximum.

Dans le cas d'un soufflet très peu conique la longeur du soufflet ouvert au max sera environ `nombre de plis × largeur des plis × 1/2`

La longeur du soufflet fermé au max sera environ `nombre de plis × épaisseur du carton × 2.5`

Pour coller le soufflet à son support, trois solutions :

1. Coller à l'exterieur du cadre
2. Coller à l'interieur du cadre
3. Coller à plat

Sur le dessin ci dessous la longueur représentée par la flèche désigne ce qu'on appelle la taille du cadre. N.b. selon la manière de coller, ce que l'on désigne par taille du cadre peut faire référence à l'interieur du soufflet (rectangle a travers le quel on regarde) ou faire référence à l'exterieur du soufflet (encombrement du soufflet quand il est plié)

![schema collage soufflet](/contenu/plans/collage-soufflet.svg)

### Dessin

On va d'abord dessiner une arette du soufflet (un quart du soufflet) puis la dupliquer en appliquant des symetries axiales pour avoir le soufflet complet.

#### Tracer le pli en zigzag de l'arette

On commence par tracer deux traits verticaux espacé de la largeur d'un pli puis on trace un zigzag entre ces deux traits avec des angles de 90°. Ce zigzag a autant de sommets qu'il y aura de plis.

#### Tracer la médianne du pan de gauche

Soit C et D les deux extrémités du zigzag.

Tracer un cercle de centre C.
Si le trait du zigzag qui part de C va vers la gauche, le diamètre du cercle est `longueur du **petit** côté du **petit** cadre + largeur des plis`.
Sinon le diamètre est la longueur du **petit** côté du **petit** cadre.

Tracer un cercle de centre D.
Si le trait du zigzag qui part de D va vers la gauche, le diamètre du cercle est `longueur du **petit** côté du **grand** cadre + largeur des plis`.
Sinon le diamètre est la longueur du **petit** côté du **petit** cadre.

La médiane du pan de gauche est la tangeante exterieure à ces de cercle qui passe à gauche des cercles. On la note droite d.

#### Tracer les plis du pan de gauche

Soit C' L'intersection de cette droite avec le cercle de centre C et D' l'intersection de cette droite avec le cercle de centre D.

les segments CC' et DD' sont le premier et le dernier pli du pan. CC' et DD' sont parallèles.

Tous les autres plis du pans peuvent désormais être tracés, ce sont les segments parallèles à CC' par chaque sommet du zigzag. on fait aller ces segments des sommets du zigzag à la droite d

#### Reproduire ces étapes pour le pan de droite

Pour la médianne du pan de droite reproduire ces étapes symétriquement, mais en prenant en compte les longueurs des **grands** côtés des cadres.

#### Tracer les languette aux extremités du soufflet.

pour la partie ou on collera se referer à ce [schema](plans/collage-soufflet-patrons.png) en fonction de ce que l'on a choisi comme manière de coller le soufflet au cadre. (En vert les pls exterieurs en cyan les plis interieurs)

#### Dupliquer le tracé 

tracer la symétrie du dessin par la médiane du côté de gauche (droite d).

Puis tracer à nouveau la symétrie du dessin ainsi obtenu par la médiane du côté de droite.

