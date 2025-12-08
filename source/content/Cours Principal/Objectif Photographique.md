## Système optique centré

Un **système optique centré** est constitué de plusieurs lentilles, pas nécessairement minces, partageant le même [[Lentille mince#Axe optique|axe optique]]. qui constitue un axe de symétrie de révolution.

Un **objectif photographique** est un système optique centré comportant entre 5 et 8 lentilles, parfois plus. Certaines sont divergentes, mais l'ensemble doit être **convergent**, c'est-à-dire créer des [[Objectif-Subjectif (Réel-Virtuel)|images réelles (ou "objectives")]].

L'utilisation de plusieurs lentilles a plusieurs buts :
1. Permet de corriger les défauts des objectifs, appelés **aberrations**.
   Il existe 7 types d'aberrations :
	1. (Défaut géométrique radial) la **distorsion** : un grillage plat apparaît tordu
      ![Exemple de distorsion pour une simple grille (crédit: Baptiste Desnouck)](bd_distorsion.jpg)
	2. (Défaut colorimétrique) le **vignettage** : les bords de l'image apparaissent plus sombres
	3. (Défaut colorimétrique) l'**aberration chromatique** : les couleurs au bords de l'image sont décorrélées car les verres de la lentille ont un indice de réfraction qui dépend légèrement de la longueur d'onde (*effet de prisme*)
	4. (Défaut de netteté) la **courbure de champ**
	5. (Défaut de netteté) l'**astigmatisme**
	6. (Défaut de netteté) la **coma**
	7. (Défaut de netteté) l'**aberration de sphéricité**
2. Permet de fabriquer des objectifs de distance focale élevée (*"télé-objectif"*), avec un encombrement réduit.

## Éléments cardinaux d'un objectif
Un objectif possède quatre **éléments cardinaux**, qui sont quatre planes perpendiculaires à l'axe optique :
- **Deux plans focaux** : le plan focal objet $(F)$ et le plan focal image $(F')$ 
- **Deux plans principaux**, conjugués entre eux, et notés $(H)$ et $(H')$.
  Les intersections de ces plans avec l'axe optique sont :
	- $(F) \rightarrow F_0$ **foyer principal** objet
	- $(F') \rightarrow F'_0$ **foyer principal** image
	- $(H) \rightarrow H_0$ **point principal** objet
	- $(H) \rightarrow H'_0$ **point principal** image
![Schéma des éléments cardinaux (crédit: Baptiste Desnouck)](bd_el_card.jpg)
- **Deux points nodaux** $N$ et $N'$ sont deux points conjugués situés sur l'axe optique, tels que tout rayon incident passant par $N$, après traversée de l'objectif, passe par $N'$ (car $N'$ est l'image de $N$) avec la même direction que la direction initiale.
  Dans le cas où l'objectif est plongé dans l'air, ces points sont confondus avec les points principaux : $N \equiv H_0$ & $N' \equiv H'_0$
- **Distances focales** : ce sont les distances algébriques suivantes :
	- $f = \bar{NF_{0}}$, la distance focale object
	- $f' = \bar{N'F'_0}$, la distance focale image
  Si l'objectif est plongé dans l'air,
  $$f = - f'$$
  Pour un système optique centré convergent,
  $$f' \geqslant 0$$
> Dans une lentille mince, les plans principaux sont situés sur le plan moyen.
> ![Représentation graphique (crédit: Baptiste Desnouck)](bd_plan_p_m.jpg)

## Relation de [[Conjugaison (optique)|conjugaison]]
La règle de l'**aplanétisme**, déjà utilisée dans les [[Rappels d'optique géométrique#Règles de construction|rappels d'optique géométrique]] (règle #4), est encore vraie pour un objectif : les plans orthogonaux à l'axe optique sont conjugués deux à deux.

On oriente l'axe optique vers la droite et on utilise deux origines : $N$ pour l'espace object et $N'$ pour l'espace image.
![Schéma de cette relation (crédit: Baptiste Desnouck)](bd_aplan.jpg)
La **relation de conjugaison** ([[Lois de Descartes|Descartes]]) s'écrit :
$$
\tag{1}  \boxed{- \frac{1}{p} + \frac{1}{p'} = \frac{1}{f'} }
$$
Différents cas :
- $p = - \infty \implies p' = f'$ (définition du plan focal image)
- $p = f = -f' \implies \frac{1}{p'} = 0 \implies p' = +\infty$ (définition du plan focal objet)
- $p = 2f = -2f' \implies \frac{1}{p'} = \frac{1}{2f'} \implies p' = 2f' = -p$
- Règle à retenir : les plans conjugués $(P)$ et $(P')$ se déplacent dans le même sens.

## Règles de constructions des images
### Cas $p = 2f = -2f'$ :
  ![$p = 2f = -2f'$ (crédit: Baptiste Desnouck)](bd_p_2f.jpg)
0. Tout rayon passant par un point de $(H)$, après traversée de l'objectif, passe par un point de $(H')$ **de même ordonnée**. 
   C'est ce qui caractérise la paire de plans principaux.
Les autres règles sont similaires à [[Rappels d'optique géométrique#Règles de construction|celles de la lentille mince]] :
1. Tout rayon passant par $N$ sort en passant par $N'$ avec la même direction.
2. Tout rayon passant par $F_0$ sort parallèle à l'axe optique.
3. Tout rayon parallèle à l'axe optique sort en passant par $F'_0$.
Comme pour la lentille mince, il faut un autre règle pour construire l'image d'un point situé sur l'axe optique.
4. **Règle de l'aplanétisme** : $(P)$ et $(P')$ sont conjugués.
