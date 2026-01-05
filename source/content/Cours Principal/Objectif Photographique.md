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

## Centre optique d'un objectif
Le [[bd_p_2f.jpg|dessin précédent]] montre une forte analogie entre le [[Lentille mince#Centre optique|centre optique]] $O$ de la lentille mince et la pire de points nodaux $(N, N')$.
En retirant l'espace compris entre les plans $(H)$ et $(H')$, on retrouve exactement les [[bd_rc123.jpg|constructions géométriques de la lentille mince]].

![Transformation entre les constructions d'un objectif optique et d'une simple lentille mince (crédit: Baptiste Desnouck)](bd_obj_to_lent.jpg)

Le **centre optique** d'un objectif n'a pas de réalité physique. Il est confondu avec $N$ dans l'espace object, et avec $N'$ dans l'espace image.
Ce point est très souvent utilisé en vision par ordinateur. Il constitue le **centre de projection** du modèle **sténopé**, qui est une projection centrale sur le "plan image" (voir plus loin)

## Grandissements d'un objectif
⚠ **Grandissement $\neq$ grossisement**
On positionne dans le plan object $(P)$ au point $A$, un objet de "petite dimension" transverse $dy$ :
![Schéma du système (crédit: Baptiste Desnouck)](bd_gross.jpg)
D'après la [[#Règles de constructions des images|règle 4]], l'image de cet objet est contenu dans $(P')$, de taille $dy'$. On définit le **grandissement transverse** par :
$$ \tag{2} G_{\bot} = \frac{dy'}{dy} $$
D'après le théorème de Thalès :
$$ \tag{3} G_{\bot} = \frac{p'}{p} $$
En combinant $\text{(3)}$ et la [[#Relation de Conjugaison (optique) conjugaison|relation de conjugaison]] $\text{(1)}$ :
$$
\frac{1}{p'} = \frac{1}{f'} + \frac{1}{p} = \frac{p+f'}{f'p} \\
\implies \frac{p'}{p} = \frac{f'}{p+f'} \\
\implies \boxed{\tag{4} G_{\bot} = \frac{f'}{p+f'}}
$$
Comme l'objet doit se situer à gauche de $(F)$, sans quoi son image serait subjective, cela signifie que $|p| > f'$, donc $p + f' < 0$.
Par conséquent, on a toujours :
$$
G_{\bot} < 0 \tag{5}
$$
Ceci traduit le fait que les images sont inversées.

__Exemples__ :
- $p \in ]-\infty, -2f'[ \implies |G_{\bot}|<1$
- $p = -2f'\implies |G_{\bot}|=-1$
- $p \in ]-2f', -f'[ \implies |G_{\bot}|>1$

On place maintenant un objet en $A$, de dimension axiale $dp$. Son image n'est pas axiale, mais on s'intéresse à sa dimension axiale $dp'$.
On définit le **grandissement axial** par :
$$ G_{//} = \frac{dp'}{dp} \tag{6} $$
En dérivant la [[#Relation de Conjugaison (optique) conjugaison|relation de conjugaison]] :
$$
-\frac{1}{p} + \frac{1}{p'} = \frac{1}{f'} \implies \frac{dp}{p^2} - \frac{dp'}{p'^2} = 0 \\
\implies \frac{dp'}{dp} = \frac{p'^2}{p^2} \\
\implies \boxed{G_{//} = \left( \frac{p'}{p} \right)^2 \tag{7}}
$$
On voit que $G_{//} > 0$, ce qui confirme que l'objet et son image se déplacent dans la même direction.

## Modèle sténopé et mise au point
De $\text{(3)}$ et $\text{7}$, on tire la relation suivante :
$$
\boxed{G_{//} = G_{\bot}^2} \tag{8}
$$
Cette relation est fondamentale en photographie. Elle signifie que l'image ne respecte pas les proportions de l'objet.

En photographie "macroscopique" (usuelle), l'objet est de l'ordre du mètre, alors que l'image est de l'ordre du centimètre (dimension standard du capteur : $24mm \times 36mm$).
Par conséquent :
$$
|G_{\bot}| \approx \frac{1}{100} \implies G_{//} = G_{\bot}^2 = \frac{1}{10000} \\
\implies \boxed{G_{//} \ll G_{\bot}} \tag{9}
$$

![Exemple d'une roue de tracteur (crédit: Baptiste Desnouck)](bd_pneu.jpg)

À partir d'un object 3D, on obtient une image 2D. On a perdu la 3e dimension. L'image est obtenue par projection centrale, de centre $C \equiv N \equiv N'$, sur un plan parallèle à l'axe optique.
D'après $\text{(4)}$ :
$$
G_{\bot} = \frac{f'}{p+f'} \approx -\frac{1}{100} \\
\implies p+f' \approx -100 f' \\
\implies p \approx -100 f' \tag{10}
$$
D'après la [[#Relation de Conjugaison (optique) conjugaison|relation de conjugaison]] :
$$
p' = \frac{pf'}{p+f'} \overset{\text{(10)}}{\implies} p' \approx f' \tag{11} 
$$

Le plan image $(P')$ est quasiment confondu avec le plan focal image $(F')$. Le **modèle sténopé** est une projection centrale de centre $C$, appelé **centre optique**, sur le plan focal image $(F')$.

## Autres cas de figure
Si l'objet photographié a une taille de l'ordre du centimètre, alors objet et image ont des dimensions du même ordre.
On déduit de $\text{(8)}$ :
$$
G_{//} \approx |G_{\bot}| \tag{12}
$$

## Faire la mise au point ("focus")
Cela consiste à déplacer le plan du récepteur photosensible du manière à le faire coïncider avec le plan image $(P')$.
> __Remarque__ : ne pas confondre mise au point et zoom, cela n'a rien à voir.

Il est impossible de faire la mise au point sur l'ensemble de l'objet. Cela provoque un flou en dehors du plan de mise au point. On est dans un cas où la "profondeur de champ" (voir suite du cours) est insuffisante.

Il existe trois sources de flou :
- **manque de profondeur de champ**
- **flou de bougé** (aussi appelé "flou de mouvement")
- **flou de mise au point**

Il n'existe pas d'appareil photographique spéciaux pour la macrophotographie. Il suffit d'ôter l'objectif et d'ajouter un tube entre boîtier et objectif.
![Schéma du boîtier avec un tube (crédit: Baptiste Desnouck)](bd_tube.jpg)

Enfin, si l'objet a une taille $\approx 100 \micro m$, alors $G_{\bot} \approx -100$, donc :
$$
G_{//} \gg |G_{\bot}| \tag{13}
$$

En **photographie microscopique**, pour qu'une image soit nette, on doit aplatir l'objet entre deux lamelles de verre.

## Ouverture d’un objectif

L'ouverture d'un objectif permet de contrôler la **clarté** de l’image. Elle est réglable, comme le temps de pose. Une caractéristique essentielle (outre la focale) est son **ouverture maximale**.
Plus elle est éclairée, plus l’objectif est cher.

**⚠️ Attention⚠️** : une ouverture 2× supérieure et un temps de pose 2× inférieur ne donnent pas la même photographie.
	- Si la scène est mobile, il y a plus de flou de bougé si le temps de pose augmente.
	- La modification de l’ouverture influe sur la **profondeur de champ**.

À la traversée de l’objectif, la lumière franchit un certain nombre de **diaphragmes**, dont les montures des lentilles.  
Un de ces diaphragmes, appelé **diaphragme d’ouverture**, est réglable à l’aide d’un système à iris :

![Schéma du diaphragme d’ouverture (crédit : Baptiste Desnouck)](dia_ouverture.jpg)

Le diaphragme d’ouverture se situe entre deux lentilles.  
L’image du diaphragme d’ouverture (DO) par la lentille avant (L\_avant) — système optique constitué des lentilles situées à l’avant du DO — s’appelle la **pupille d’entrée**, dont le diamètre est noté **D**.

La clarté de l’image d’un point objet est proportionnelle à la surface de la pupille d’entrée, donc à $D^2$.

Par ailleurs, si $D$ reste constant mais que l’on modifie la distance focale image $f'$ (objectif de type *zoom*), on rappelle que :

$$
G_{\perp} = \frac{f'}{p + f'}
$$

En photographie macroscopique :

$$
G_{\perp} = \frac{f'}{p}
$$

Donc la taille de l’image est quasiment proportionnelle à $f'$ : c’est l’intérêt d’utiliser un zoom.

La **quantité de lumière** qui forme l’image se répartit sur une surface proportionnelle à $G_{\perp}^2$, donc à $f'^2$.  
La clarté d’un point image est donc proportionnelle à $\frac{1}{f'^2}$.

En tout :

$$
\text{clarté} \sim \left( \frac{D}{f'} \right)^2 \tag{14}
$$

On appelle **nombre d’ouverture (NO)** d’un objectif :

$$
\text{NO} \sim \frac{f'}{D} \tag{15}
$$

**Attention** : la clarté croît lorsque le NO décroît.

De (14) à (15), on tire :

$$
\text{clarté} \sim \frac{1}{\text{NO}^2} \tag{16}
$$

Les valeurs de NO sont normalisées. Elles forment une suite géométrique de raison $\sqrt{2}$.

![Schéma NO (crédit : Baptiste Desnouck)](NO.jpg)

Lorsqu’on passe d’une valeur normalisée à la suivante, la clarté est divisée par  
$(\sqrt{2})^2 = 2$.

---

## Profondeur de champ

Un plan objet $(P)$ est conjugué d’un plan image $(P')$ : règle de l’aplanétisme.  
Pour un plan $(P)$ donné, *faire la mise au point* consiste à faire coïncider le plan du récepteur avec $(P')$.

Or, le récepteur peut occuper un petit intervalle de part et d’autre de $(P')$ sans que l’image soit floue : c’est la **latitude de mise au point**.

![Schéma mise au point (crédit : Baptiste Desnouck)](mise_au_point.jpg)

Si la coïncidence entre le récepteur et $(P')$ n’est pas parfaite, alors l’image d’un point  
$A \in (P)$ est une petite tache.  
Tant que cette tache est plus petite que la cellule élémentaire du récepteur, l’image reste nette.

Dans l’œil, cette taille est de l’ordre de **2 µm** (cônes et bâtonnets).

Les cellules élémentaires du récepteur sont :
- En photographie argentique : le cristal de sel d’argent.
- En photographie numérique : le pixel.

La latitude de mise au point dépend :
- de la focale $f'$ de l’objectif,
- du diamètre $D$ de sa pupille d’entrée,
- de la position $p$ de l’objet,
- de la nature du récepteur.

La notion de **profondeur de champ** est liée à celle de latitude de mise au point, mais de manière « inverse ».

Ici, le récepteur est fixe en un plan $(P')$, et le plan objet conjugué $(P)$ peut se situer entre deux positions extrêmes $(P_1)$ et $(P_2)$ sans que l’image devienne floue.  
La profondeur de champ est la distance entre $(P_1)$ et $(P_2)$.


![Schéma profondeur de champ (crédit : Baptiste Desnouck)](profondeur_champ.jpg)

### Remarques

- Se méfier des règles toutes faites du type : *« La profondeur de champ croît lorsque… »*
- Si tout le reste est fixe, la profondeur de champ croît lorsque le NO croît.
- Pour faire la mise au point, on a intérêt à diminuer la profondeur de champ.

---

## Angle de champ

Le **champ** d’un objectif désigne la partie de l’espace objet qui sera enregistrée sur la photographie.  
Comme pour la profondeur de champ, la notion de champ fait intervenir à la fois l’objectif et le récepteur.

- La profondeur de champ désigne en fait la *profondeur de champ net*.  
  En dehors de l’espace $(P_1)$–$(P_2)$, les points objets ont une image floue.

![Schéma angle de champ (crédit : Baptiste Desnouck)](angle_champ.jpg)

- L’angle $\alpha_c$ est l’**angle de champ**.  
  Celui de l’œil humain est d’environ **46°**.  
  Un objectif est dit **standard** si son angle de champ est du même ordre.

Comme la dimension standard du récepteur est **24 mm × 36 mm** :

![Calcul dimension récepteur (crédit : Baptiste Desnouck)](calc_angle_champ.jpg)

$$
\tan\left(\frac{\alpha_c}{2}\right) = \frac{d_{\text{max}}}{p'} \approx \frac{d_{\text{max}}}{f'}
$$

$$
f' = \frac{d_{\text{max}}}{\tan\left(\frac{\alpha_c}{2}\right)}
= \frac{21{,}6}{\tan 23^\circ} \approx 50{,}9\ \text{mm}
$$

- Si $f'$ diminue, l’angle de champ $\alpha_c$ augmente : **objectif grand angle** (ex. : 35 mm).
- Si $f'$ augmente, $\alpha_c$ diminue : **téléobjectif** (ex. : 85 mm).

L’intérêt d’agrandir le champ est évident (ex. : *fish-eye*).  
En revanche, on ne voit pas immédiatement l’intérêt à diminuer le champ, mais c’est le seul moyen d’agrandir l’image.