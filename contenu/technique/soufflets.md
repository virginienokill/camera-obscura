# Les soufflets

Pour effectuer la mise au point et lorsque l'on change de focale, il faut changer la distance entre l'écran et l'optique.
Or, quelque soit la position de l'optique par rapport à l'écran, il faut que la chambre reste hermétique à la lumière.

Pour concilier étanchéité du dispositif et possibilité varier la position relative des deux parties,
la solution traditionnellement utilisée pour les chambres noires photographiques (mais aussi pour les accordéons et les autobus articulés) est celle du soufflet.

Bien que le choix du soufflet vienne apporter une solution très satisfaisante au problème décrit ci-dessus, il apporte aussi son lot de soucis :
- Le patron d'un soufflet est difficile à dessiner.
- Le choix des matériaux est délicat (robustesse, souplesse, étanchéité, couleur)
- La construction d'un soufflet est chronophage.

<div style="padding-bottom: 56.25%; max-width: 100%; position: relative;"><iframe src="https://player.vimeo.com/video/816255116?title=0&portrait=0&byline=0" width="800px" height="450px" style="position: absolute; top: 0px; left: 0px; width: 100%; height: 100%;" frameborder="0"></iframe></div>

*Timelapse de la construction d'un soufflet pour la [camera 03](../prototypes/camera03.md)*

![animation maquette soufflet](/contenu/img/animation-maquette-soufflet-a.gif)
![animation maquette soufflet](/contenu/img/animation-maquette-soufflet-b.gif)

*Maquette de soufflet en papier*



## Processus de fabrication

### Dessiner un soufflet

On s'intéresse ici à la construction de soufflets "coniques" et "rectangulaires".

![patron d'un soufflet](/contenu/plans/soufflet-cam03-A.png)

*Exemple de patron d'un soufflet*

### Préparation

Choix à faire avant de commencer :

- taille du grand cadre
- taille du petit cadre (côté objectif)
- largeur des plis
- nombre de plis
- La manière dont le soufflet est collé au grand cadre et au petit cadre.

Pour la largeur des plis on choisit en général 100mm ou 50mm. Puisque le soufflet est conique les plis mesureront une fois sur deux un peu plus et une fois sur deux un peu moins que la valeur choisie. Cette valeur est néanmoins très importante pour dessiner le soufflet.

Le nombre de plis déterminera la longueur du soufflet minimum et maximum.

Dans le cas d'un soufflet très peu conique la longueur du soufflet ouvert au max sera environ `nombre de plis × largeur des plis × 1/2`

La longueur du soufflet fermé au max sera environ `nombre de plis × épaisseur du carton × 2.5`

Pour coller le soufflet à son support, trois solutions :

1. Coller à l'extérieur du cadre
2. Coller à l'intérieur du cadre
3. Coller à plat

**Attention : il est possible qu'une erreur se soit glissée dans les instructions concernant les collages 2 et 3**

Sur le dessin ci-dessous la longueur représentée par la flèche désigne ce qu'on appelle la taille du cadre. N.b. selon la manière de coller, ce que l'on désigne par taille du cadre peut faire référence à l'intérieur du soufflet (rectangle à travers lequel on regarde) ou faire référence à l'extérieur du soufflet (encombrement du soufflet quand il est plié)

![schema collage soufflet](/contenu/plans/collage-soufflet.svg)

### Dessin

On va d'abord dessiner une arête du soufflet (un quart du soufflet) puis la dupliquer en appliquant des symétries axiales pour avoir le soufflet complet.

#### Tracer le pli en zigzag de l'arête

On commence par tracer deux traits verticaux espacés de la largeur d'un pli puis on trace un zigzag entre ces deux traits avec des angles de 90°. Ce zigzag a autant de sommets qu'il y aura de plis.

#### Tracer la médiane du pan de gauche

Soit C et D les deux extrémités du zigzag.

Tracer un cercle de centre C.
Si le trait du zigzag qui part de C va vers la gauche, le diamètre du cercle est : *1/2 × longueur du **petit** côté du **petit** cadre + largeur des plis*.
Sinon le diamètre est *1/2 × longueur du **petit** côté du **petit** cadre*.

Tracer un cercle de centre D.
Si le trait du zigzag qui part de D va vers la gauche, le diamètre du cercle est *1/2 × longueur du **petit** côté du **grand** cadre + largeur des plis*.
Sinon le diamètre est *1/2 × longueur du **petit** côté du **grand** cadre*

La médiane du pan de gauche est la tangeante extérieure à ces deux cercles qui passe à gauche des cercles. On la note droite d.

#### Tracer les plis du pan de gauche

Soit C' l'intersection de cette droite avec le cercle de centre C et D' l'intersection de cette droite avec le cercle de centre D.

les segments CC' et DD' sont le premier et le dernier pli du pan. CC' et DD' sont parallèles.

Tous les autres plis du pan peuvent désormais être tracés, ce sont les segments parallèles à CC' par chaque sommet du zigzag. on fait aller ces segments des sommets du zigzag à la droite d.

#### Reproduire ces étapes pour le pan de droite

Pour la médiane du pan de droite reproduire ces étapes symétriquement, mais en prenant en compte les longueurs des **grands** côtés des cadres.

#### Tracer les languettes aux extremités du soufflet.

pour la jonction cadre-soufflet se référer à ce [schema](/contenu/plans/collage-soufflet-patrons.png) en fonction de ce que l'on choisit comme manière de coller le soufflet au cadre. (En vert les plis extérieurs en cyan les plis intérieurs)

#### Dupliquer le tracé 

tracer la symétrie du dessin par la médiane du côté de gauche (droite d).

Puis tracer à nouveau la symétrie du dessin ainsi obtenu par la médiane du côté de droite.

## Construire un soufflet

Le soufflet sera réalisé avec un sandwich tissu-carton-skaï :
- Du tissu noir à l'intérieur
- Du carton 1mm pour la rigidité.
- Du skaï blanc à l'extérieur pour la fraicheur et l'étanchéité.

Le carton est coupé à la découpeuse laser : on creuse une gouttière de 2.5mm entre chaque pan et on laisse un petit raccord de 2.5mm tous les 200mm pour conserver la forme sans gêner le pliage.

La découpeuse laser du FabLab de Graulhet nous permet de découper des plaques en carton de 1000x700mm

Les fichiers pour la découpe seront fournis au format dxf.

Le sandwich est collé à la colle à reliure, temps de séchage = 24h.
