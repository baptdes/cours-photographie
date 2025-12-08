# Généralités

Deux éléments :

- le boîtier
  - le capteur
  - le [[#Le viseur|viseur]]
  - l'[[#L'obturateur|obturateur]]
- l'[[Objectif Photographique|objectif]]

## Le viseur

- Permet d'avoir une idée de l'image qui sera enregistrée
- Deux types de viseurs :
  - viseurs "à travers l'objectif" (*TTL* en anglois, *"Through The Lens"*), dont deux sous-types
    Dans les deux cas, l'image formée dans le viseurs traverse l'objectif, donc il n'y aura **pas de déformation entre cette image et l'image enregistrée**.
    - viseurs sur écran
    - viseurs *reflex*, plus fiable du point de vue colorimétrique
      Une caractéristique de la visée *reflex* (visée utilisée par tous les professionnels) est qu'il y a **un miroir qui pivote au moment de la prise de vue** (plutôt difficile à mettre en œuvre...)
      ![Un petit schéma du système *reflex* (crédit: Baptiste Desnouck)](bd_schéma_reflex.jpg)
      mais il y a des inconvénients !
      - encombrant
      - lourd
      - fragile
      - le pivotement du miroir fait du bruit (gênant lors d'un spectacle)
        *"Sauf si c'est du hard rock, là, ça va" - Jean-Denis Durou*
      - cela provoque aussi de légères vibrations, gênant en photographie scientifique (ex: stéréophotométrie)
  - viseurs optiques
    - Les viseurs optiques utilisent un système optique secondaire
      ![Schéma d'un viseur optique - on voit le système secondaire! (crédit: Baptiste Desnouck)](bd_schéma_viseur_optique.jpg)
      Cela cause une déformation géométrique appelée "parallaxe"          ![Example de parallaxe quand l'appareil est trop proche du sujet (crédit: Paul Bourke)](https://paulbourke.net/miscellaneous/parallaxerror/9cm.jpg)

## Les 4 gammes d'appareils

Il existent quatre gammes, qui sont caractérisées par le type de visée et la possibilité ou non de changer l'objectif.

|                          | TTL (*reflex*)   | TTL (écran)  | Optique          |
| ------------------------ | ---------------- | ------------ | ---------------- |
| **Objectif<br>amovible** | 1. *Reflex*      | 2. *Hybride* | Existe pas<br>:( |
| **Objectif<br>fixe**     | Existe pas<br>:( | 3. Bridge    | 4. Compact       |

Avant l'ère du numérique, il n'existait que le *reflex* et le compact.

## L'obturateur

L'obturateur permet de laisser passer la lumière vers le capteur que pendant un laps de temps appelé "temps de pose", ou "temps d'exposition". Rien à voir avec la [[café?.png|pause café]].

Il existe trois types :

- Obturateur à iris (désuet)
- Obturateur à rideau
  Comporte deux rideaux opaques qui défilent devant le capteur avec un décalage $\Delta t =$ temps de pose
  ![Schéma de l'obturateur à rideau (crédit: Baptiste Desnouck)](bd_obturateur_rideau.jpg)
  L'interêt est que tous les points du capteur sont exposés à la lumière pendant la même durée $\Delta t$, mais il y a un décalage temporel entre les différents points. Cela peut causer des déformations d'objets en mouvement.
  ![Example de déformation des roues d'une voiture (crédit: Jacques Henri Lartigue)](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fcdn.britannica.com%2F42%2F196342-050-02682FEC%2FGrand-Prix-ACF-Dieppe-photograph-Jacques-Henri-Lartigue-1912-Yale-University-Art-Gallery.jpg&f=1&nofb=1&ipt=b632ba090526697e2558acdf89d0d306e200063c1b79639c417398c2a72d919a)
- Obturateur éléctronique
  ⚠ L'obturateur éléctronique n'équipe pas tous les appareils numériques !
  Cet obturateur présente trois avantages :
  - Tous les pixels sont exposés à la lumière pendant le même temps, et la même durée, et **sans décalage !**
  - Évite les bruits et vibrations causés par les obturateurs mécaniques
  - Permet d'atteindre des temps de pose très courts, là où les obturateurs mécaniques ne peuvent pas

Les temps de pose peuvent prendre des valeurs prédéfinies :
$$\Delta t \in [\underbrace{1s,\frac{1}{2}s,...,\frac{1}{100}s,...,\frac{1}{1000}s}_\text{obturateurs mécanique},...,\frac{1}{32000}s]$$

Il y a deux types de pose longue :

- B : temps d'appui sur le déclencheur
- T : deux appuis successifs début/fin