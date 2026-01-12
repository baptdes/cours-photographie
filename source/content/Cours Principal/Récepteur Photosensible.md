## Intro : l'œil humain
On classe les fréquences électromagnétiques en fonction de la longueur d'onde dans le vide.
![Le spectre de la lumière selon la longueur d'onde (crédit: Baptiste Desnouck)](bd_wavelengths.jpg)

Entre ultraviolets et infrarouge, il existe une mince bande de fréquences visibles : le **"spectre lumineux"** ou **"spectre visible"**.
En réalité, l’œil n'est pas uniformément sensible dans ce domaine. On a établi expérimentalement la **courbe de visibilité** de l'œil humain moyen, qui diffère entre jour et nuit. Ces deux courbes qui ont une allure gaussienne, sont décalées.
![Les courbes de visibilité de l'œil humain (crédit: Baptiste Desnouck)](bd_courbe_visibilite.jpg)

Le vert, à 555nm, est aussi le maximum de puissance de la lumière du Soleil (au sol). C'est une illustration de l'adaptation.
Dans l'œil, le récepteur photosensible est la rétine, qui comporte deux types de **cellules photosensible** : bâtonnets et cônes, de dimensions autour de 4µm. Cette nature discontinue est à l'origine du **pouvoir séparateur** fini de l'œil : dimension minimale de deux points image pouvant être distingués (on parle aussi de **pouvoir de résolution**).

## Qu'est-ce qu'une bonne photographie ?
C'est une photo qui doit être "indiscernable" de la scène 3D photographique. Une telle transformation est dite **"idempotente"**.
Cette propriété concerne la **géométrie** et la **photométrie**.
Pour la géométrie, on a déjà vu que la distance focale "standard" correspond au même angle de champ que l'œil humain. Cela signifie que les téléobjectifs et les objectifs grand angle (voir [[Objectif Photographique#Angle de champ|la partie du cours sur l'angle de champ]]) déforment la perception de la scène 3D:
![Apparence des objets selon les objectifs (crédit: Baptiste Desnouck)](bd_angle_objectifs.jpg)

Pour la **photométrie** (couleur des objets), une photo doit être fidèle à l'original. Pour cela, il existe en photographie numérique une fonction de **balance des blancs** automatique. Il est cependant encore plus efficace d'utiliser une **charte colorimétrique.**
> "Le club photo est riche!" - Jean-Denis Durou

## Photographie Argentique
Le récepteur de la photographie argentique en noir & blanc est constitué d'un support (verre, film souple ou papier) sur lequel a été déposée une fine couche d'**émulsion** ("comme la mayonnaise" - Jean-Denis Durou), qui est une suspension de cristaux d'**AgBr** (soit de **[bromure d'argent](https://fr.wikipedia.org/wiki/Bromure_d'argent)**) dans un liant de gélatine. On a encore ici un récepteur de nature discontinue.
L'exposition à la lumière crée une "image latente" invisible : cristaux d'AgBr qui ont absorbé des photons lumineux, par opposition à ceux qui n'en ont pas absorbé.

Le **développement** procède en plusieurs étapes :
- Dans une chambre noire, le **révélateur**, par une réaction chimique de "réduction", transforme les cristaux d'AgBr ayant absorbé des photons en "grains" d'argent métallique, qui est noir.
- Le **fixateur** élimine les cristaux d'AgBr résiduels.
- Après rinçage à l'eau et séchage, on obtient une **image en noir et blanc négative**.
- À partir du négatif, en utilisant un **agrandisseur**, on obtient un **image en noir et blanc positive** en répétant l'opération.

La sensibilité de l'émulsion dépend de la longueur d'onde. Naturellement, elle est sensible au bleu-violet. En ajoutant des colorants appropriés, on la rend sensible à l'ensemble du spectre  visible : on parle d'**émulsion panchromatique**.

Pour la photographie argentique en couleur, on doit utiliser des filtres colorés (voir suite du cours (TODO))

On définit la **densité optique** du récepteur argentique après développement par :
$$
D = -\log\frac{\varphi'}{\varphi}
$$
![Flux lumineux caractérisants de la densité optique (crédit: Baptiste Desnouck)](bd_varphi.jpg)
On définit aussi l'**exposition lumineuse** :
$$
H = ET
$$
où $E$ est l'éclairement et $T$ le temps de pose.

Un récepteur argentique est caractérisé par la **courbe de Hunter et Driffield**.
![Example d'une courbe de Hunter et Driffield (crédit: Baptiste Desnouck)](bd_hunter_driffield.jpg)

On s'arrange pour se situer dans la zone 2 :
$$
D = A + \gamma \log H
$$
La pente $\gamma$ est appelée le "gamma" de l'émulsion. La **sensibilité** d'un film argentique en ISO (100 ISO, 200 ISO, ..., 1600 ISO) est proportionnelle à $\gamma$ . Un film est plus sensible si les cristaux d'AgBr sont plus gros.