En photographie numérique, il existe deux types de récepteurs  photosensibles :
- **CCD** (*charge coupled device*), inventé en 1969 par deux ingénieurs de AT&T et Bell.
- **CMOS** (*complementary metal oxyde semiconductor*) inventé en 1990 par Eric Fossum, en collaboration avec la NASA.
Ces deux technologies reposent sur le même principe : _l'effet photoélectrique_ qui transforme les photons en charge électrique.

Remarques : 
- Dans une LED, c'est le phénomène inverse qui se produit
- Dans $E = h * \nu$, un photon violet est plus énergétique qu'un photon rouge.

A l'heure actuelle, le CMOS a quasiment remplacé le CCD pour des raisons de cout de fabrication.
Plus le récepteur est grand, plus il est cher. Il n'existe pas de format standard, mais on se réfère toujours au format standard de l'argentique 24x36 de l'argentique.

Les récepteurs électroniques ont tous une taille $\le$ à 24mm x 36mm

![Schéma récepteur électronique (crédit: Timothée Klein)](recepteur_elec.png)

On dit d'un appareil numérique qu'il a une focale _équivalent 24x36_ si sont angle de champ est celui de l'oeil humain (46°), quelle que soit la dimension du récepteur.

Le rapport 2/3 du 24x36 entre largeur et hauteur a été remis en question en photo numérique :
- 2/3
- 3/4
- 9/16
- ...

En photo argentique, la taille des récepteurs élémentaires (cristaux d'AgBr), qui définit la résolution, est liée à la sensibilité du film.
En photo numérique, la résolution (liée à la taille du pixel) est indépendante de la sensibilité.

La courbe de Hunter et Driffield est remplacé en ordonnée, par une tension électrique. Elle est beaucoup plus linéaire, mais : 
- Pour les valeurs très faibles, le signal est noyé dans le bruit (*thermique*) PSNR très faible.
- Pour les valeurs élevées, il y a un phénomène de saturation.

La dimension de la cellule photosensible élémentaire (pixel) est du même ordre que celle de l'oeil humain. Pour un récepteur  24x36 réel, avec des pixels carrés de dimension 4 ${\mu}m$, le nombre de pixels vaut : $\frac{24 * 36}{(4 * 10^{-3})^2} = 54 * 10^6$

En photo numérique couleur, il existe deux systèmes : 
- Un récepteur par canal coloré : _tri-CCD_ ou _tri-CMOS_ 
	On sépare le faisceau lumineux en trois faisceaux à l'aide le prismes : ![Schéma prisme (crédit: Timothée Klein)](prisme.png)
	Ce système est couteux (trois récepteurs) et lourd à cause du prisme

L'avantage est que chaque pixel possède trois valeurs numériques, contrairement au deuxième système :
- Une mosaique de filtres colorés placée devant le récepteur : un filtre coloré par pixel. La mosaique la plus classique est celle de Bayer, dont le motif est :
	![Schéma Bayer (Source : https://www.researchgate.net/publication/4087683/figure/fig1/AS:669077211213839@1536531846215/Typical-Bayer-mosaic-for-color-image-capture-in-single-CCD-digital-cameras-the-G.png)](bayer.png)
	Le vert est deux fois plus représenté car c'est le maximum de sensibilité de l'oeil.
Au format RAW, on dispose d'une seule valeur numérique par pixel. Les deux valeurs manquantes peuvent être calculées par le procédé du **démosaïquage** (par exemple par interpolation).
