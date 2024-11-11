# CAP Elec 1.46 Chute de tension
## Foley Services Elec - [Programme 2ème partie](../2eme_partie/README.md)

### 1.46 Chute de tension

- **Accès à la vidéo** [1.46 Chute de tension](https://youtu.be/9riZqBhiBao)

#### Conducteurs et résistance

Un conducteur présente intrinsèquement une résistivité (résistance) (à la circulation du courant), cette résistance multiplié par l'intensité du courant qui circule ($$U = R \cdot I$$) correspond à une tension qui est *perdue*.

Cette perte dépend de la longueur du câble utilisé.

*Analogie*: perte de pression dans un tuyau d'arrosage. La perte de pression est plus importante si on réduit la section du tuyau. A l'inverse on réduit cette perte si on uitlise une plus grande section (et plus forte pression).

- Chute de tension entre AGCP (alimentation Enedis) et l'habitation, qui se situe disons 100m plus loin.
- L'intensité a un impact direct sur la chute de tension, qui lui est proportionnelle ($$U = R \cdot I$$).
- La chute de tension dépend de la longueur $$L$$ du conducteur. *Attention*, en monophasé, on double cette longueur ($$= 2L$$)  pour tenir compte de la phase ***et*** du neutre.
- Résistivité du cuivre $$\rho_{Cu} = 0.022 \Omega / m / mm^2$$ (Ohm par mètre par mm^2), qui dépend donc à la fois de la longueur du conducteur et de sa section.
- Résistivité de l'aluminium $$\rho_{Al} = 0.036 \Omega / m / mm^2$$ (Ohm par mètre par mm^2)

Ainsi, la chute de tension se calcule en faisant le produit

$$U = R \cdot I = \big( \frac{2L \cdot \rho}{S} \big) \cdot I$$

où $$\rho$$ ets le coefficient de résistivité, $$L$$ ets la longueur du câble (doublée en raison de la présence de la phase et du neutre), divisé par la section du câble.

AInsi, dans le cas du câble de $$L =100m$$ de cuivre, de section $$S = 16mm2$$, alimenté depuis l'AGCP en $$I = 60A$$, on obtient une chute de tension:

$$U = \big( \frac{2L \cdot \rho}{S} \big) \cdot I = \frac{200 \times 0.022 \times 60}{16} = 16.5V$$

#### Seuil d'acceptabilité

Dans une installation, la chute de tension est encadrée

- 3% sur un circuit d'éclairage
- 5% sur les autres circuits

On peut modifier la chute de tension en agissant sur la section du conducteur:

$$S = \frac{2L \cdot \rho \cdot I}{U}$$

où $$U$$ est la chute de tension maximum autorisée.

Ainsi, pour une chuite de tension maximum autorisée de 6.9V (= 3% de 230V), sur une distance de 100m depuis l'habitation (donc $$L = 200m$$), AGCP 60A:

$$S = \frac{200 \times 0.022 \times 60}{6.9} = 38.26$$

et on doit donc prendre une section de 50mm2.

Si on utilise plutôt un conducteur en aluminium:

$$S = \frac{200 \times 0.036 \times 60}{6.9} = 62.6$$

et on doit donc prendre une section de 70mm2.

#### Alu ou cuivre ?

- Comparaison des prix (fonction de la distance, exemple 100m en conducteur 1 fils ou 50m en conducteur 2 fils) et de la section.
- Achat d'adaptateur pour pouvoir connecter les fils qui arrivent au tableau
  - Cuivre adaptateur 50 -> 35 ou 16
  - Alu adaptateur 70 ALu -> 50 cuivre, cuivre 50 -> 16



 