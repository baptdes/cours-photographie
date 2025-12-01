L'optique géométrique est fondée sur la notion de [[Rayon (optique)|rayon lumineux]], par opposition à l'optique physique.

## Quelques rappels
- Un milieu transparent est caractérisé par son [[Indice de réfraction]].
- On appelle **dioptre** la surface de séparation entre deux milieux transparents homogènes, d'indices $n_1$ et $n_2$ différents. À la traversée d'un dioptre, un [[Rayon (optique)|rayon]] est dévié. C'est le phénomène de [[Réfraction|réfraction]] ($\not=$ diffraction), exprimée par la [[Lois de Descartes#2ème Loi|2ème Loi de Descartes]].
- Sans la [[Réfraction|réfraction]], il serait impossible de créer des images. En effet, un [[Points objet-image#Point object|point objet]], qui est une source lumineuse de petite dimension, émet de la lumière dans toutes les directions. Sans [[Réfraction|réfraction]], ces [[Rayon (optique)|rayons]] ne se croiseraient jamais plus.
	- Avec la [[Réfraction|réfraction]], on peut faire converger ces [[Rayon (optique)|rayons]] en un autre point appelé [[Points objet-image#Point image|point image]].

## La lentille mince
Voir la notion de [[Lentille mince|lentille mince]].

## Conventions
On fait aller la lumière de la gauche vers la droite.
On appelle **espace object** le demi-espace situé à gauche de la lentille, et **espace image** l'autre demi-espace.

## Règles de construction
1. Tout [[Rayon (optique)|rayon]] passant par le [[Lentille mince#Centre optique|centre optique]] $O$ n'est pas dévié.
   ![Un rayon qui passe au centre d'une lentille n'est pas dévié (crédit: Baptiste Desnouck)](bd_rc1.jpg)
2. Tout rayon passant par le [[Lentille mince#Foyers|foyer objet]] $F$ sont parallèle à l'axe optique.
3. Tout rayon parallèle à l'[[Lentille mince#Axe optique|axe optique]] passe par le [[Lentille mince#Foyers|foyer image]] $F'$.

__Exemple avec une lentille convergente__ :
![Application des trois règles (crédit: Baptiste Desnouck)](bd_rc123.jpg)

Avec ces trois règles, il est impossible de construire l'image d'un point situé sur l'axe optique...
Heureusement, il existe une quatrième règle :
4. Les plans $(P)$ et $(P')$, passant par $A$ et $A'$, et orthogonaux à l'[[Lentille mince#Axe optique|axe optique]], sont [[Conjugaison (optique)|conjugués]], soit que tout [[Points objet-image#Point object|point objet]] situé sur $(P)$ a son image sur $(P')$.
   Ainsi, pour construire l'image d'un point $A$ situé sur le même **plan objet $(P)$**, on construit l'image $A'$ de $A$, et l'image $B'$ de $B$ se trouve sur le même **plan image $(P')$** que $A'$.

__Exemple avec une lentille divergente__ :
![Exemple (crédit: Baptiste Desnouck)](bd_rc1234.jpg)

## Remarques
- On utilise des échelles différentes selon les deux directions, c'est-à-dire selon les directions horizontales et verticales — évidemment, la distance d'un objet à une lentille n'est pas comparable au diamètre de la lentille. Cela permet d'éviter les erreurs de tracés.
- L'image $A'$ d'un point $A$ à travers une lentille **divergente** est **subjective/virtuelle** car il ne s'y concentre pas d'énergie lumineuse. Ainsi, on ne peut pas faire de photographie avec une image subjective/virtuelle !
  Au contraire, l'image de $A$ par une lentille **convergente** est **objective/réelle**. Pour cette raison, on appelle "objectif" un système optique capable de former des images objectives.