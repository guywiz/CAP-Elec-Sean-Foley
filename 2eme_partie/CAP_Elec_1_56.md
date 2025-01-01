# CAP Elec 1.56 Rappel chute de tension
## Foley Services Elec - [Programme 2ème partie](../2eme_partie/README.md)

### 1.56 Rappel chute de tension

- **Accès à la vidéo** [1.56 Rappel chute de tension](https://youtu.be/QUgGy3fLktY)

On cherche à mesurer la chute de tension dans un câble, en se basant sur la loi de Ohm $U = RI$

- On considère une intensité égale à celle qui est fournie au niveau de l'AGCP (abonnement)
- La résistance induite par le câble dépend
  - De la matière utlisée (cuivre Cu ou aluminium Al) et plus précisément de sa résistivité
  - De sa longueur (plus long $\to$ *plus* de résistance)
  - De sa section (plus grande $\to$ *moins* de résistance)


Coefficient de résistivité (exprimée en $\Omega \cdot mm^2 / m$)

- Cuivre: 0.0225
- ALuminium: 0.036

La résistance induite est

- proportinnelle à la longueur du câble: attention à tenir compte de l'aller-retour (phase/neutre) dans le câble
- inversement proportionnelle à la section du câble

Calcul de la chute de tension induite d'un câble de longueur $L$, de section $S$ et de résistivité $\rho$ (cuivre ou aluminium)

$$
U = R \cdot I\\
= (\frac{2L \cdot \rho}{S}) \cdot I
$$

(où la longueur $2L$ tient compte de l'aller-retour sur phase et neutre en situaiton monophasée).

#### Quelle section pour une chute de tension admise maximum $U$ ?

$$
S = (\frac{2L \cdot \rho}{U}) \cdot I
$$

Rappel, chute de tension maximum admise:

- 3% (d'une tension nominale 230V) sur un circuit éclairage = 6.9V
- 5% sur les autres circuits = 11.5V

#### Calcul de puissance

En situation de courant alternatif monophasé, à cause de réactance des appareils, il faut tenir compte d'un déphasage (un angle $\varphi$) du courant, et calculer la puissance active:

$$P = U \cdot I \cdot \cos \varphi$$

d'où le calcul de l'intensité

$$I = \frac{P}{U \cdot \cos \varphi}$$
