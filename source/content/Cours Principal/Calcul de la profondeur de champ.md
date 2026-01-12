> ⚠️ **Attention**  
> Se méfier des règles toutes faites : *« la PC croît lorsque … »*
> ![Schéma règle préfaites (crédit: Timothée Klein)](regle_pre_pc.png)
## Hypothèse de simplification

Pour simplifier les calculs, on suppose que la **pupille d’entrée** $P_e$ se trouve dans le **plan principal objet** $H$ :

![Schéma PC (crédit : Timothée Klein)](schema_pc.png)

## Calcul de $d_+$

![Calcul de $d_+$ (crédit : Timothée Klein)](calcul_d_plus.png)

D’après Thalès :

$$
\frac{\tfrac{t}{2}}{d_+}
= \frac{\tfrac{D}{2}}{p' + d_+}
= \frac{\tfrac{D}{2} - \tfrac{t}{2}}{p'}
$$

Comme $t \ll D$, on obtient :

$$
d_+ = \frac{t}{D}\, p'
$$

## Calcul de $d_-$

![Calcul de $d_-$ (crédit : Timothée Klein)](calcul_d_moins.png)

D’après Thalès :

$$
\frac{\tfrac{t}{2}}{d_-}
= \frac{\tfrac{D}{2}}{p' + d_-}
= \frac{\tfrac{D}{2} + \tfrac{t}{2}}{p'}
$$

Comme $t \ll D$, on obtient également :

$$
d_- = \frac{t}{D}\, p'
$$

## Expression de la profondeur de champ

Par conséquent :

$$
PC = A_-A_+ = \frac{d_- + d_+}{G_\parallel}
= \frac{2t}{D}\,\frac{p'}{G_\parallel}
\qquad (3)
$$

Or :

$$
G_\parallel = G_\perp^{\,2}
= \left(\frac{f'}{p + f'}\right)^2
\qquad (4)
$$

## Cas de la photographie macroscopique

En photographie macroscopique :

$$
|p| \gg f' \quad \text{et} \quad p' \simeq f'
$$

À partir de (3), (4) et de ces hypothèses, on obtient :

$$
PC = \frac{2t}{D}\, f'\left(\frac{p}{f'}\right)^2
= \frac{2t}{D}\,\frac{p^2}{f'}
$$

soit encore :

$$
PC = 2t\, \text{NO} \left(\frac{p}{f'}\right)^2
$$

- Si $p$ et $D$ sont constants, alors **la profondeur de champ décroît lorsque $f'$ croît**.
- Si $G_\perp$ et $D$ sont constants, alors **la profondeur de champ croît lorsque $f'$ croît**.

👉 Il faut donc **bien se méfier des règles toutes faites**.