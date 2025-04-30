# CAP 1.74 Indus 2 : démarrage directe
## Foley Services Elec - [Programme 2ème partie](../2eme_partie/README.md)

### 1.74 Indus 2 : démarrage directe

- **Accès à la vidéo** [1.74 Indus 2 : démarrage directe](https://youtu.be/anSNjzBhB5g)

#### Circuit de puissance moteur, circuit de commande

[On a déjà exposé le circuit de puissance du moteur, avec explication du rôle de chaque composante protégeant le circuit.](./CAP_Elec_1_73.md)

<img src="./images/Circuit_puissance_moteur.png" width="600">

Le circuit de commandes est alimenté en repiquant depuis uneou deux phases en amont du circuit de puissance.

Les commandes - pour des raisons de sécurité (risque de contact direct) - fonctionnent souvent sous une tension de 24V. Il faut donc utiliser un transformateur qui nous fait passer de 400V à 24V

- Le transformateur créée un appel de courant relativeemnt fort au démarrage, il faut donc protégéer le circuit à l'aide d'un sectionneur à fusible sur chacune des phases.
- - On protège avec des fuisibles de 4A, si par exemple le transformateur a une puissance de 240W (puisque $240 W \geq 400V \cdot 4A = 1600W$.

