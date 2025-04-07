# CAP Elec 1.83 Mise en service cours
## Foley Services Elec - [Programme 2ème partie](../2eme_partie/README.md)

### 1.83 Mise en service cours

- **Accès à la vidéo** [1.83 Mise en service cours](https://youtu.be/wNK_aQaREA4)

#### Mise en service (domestique)

- Scénario retenu, installation tétra (petit tertiaire).
- La mise en service concerne un tableau électrique éventuellement conçu par un tiers.

- Tableau deux rangées (minimum deux interrupteurs différentiels en domestique)

#### Principes de l'exercice de mise en service

- Protection individuelle
  - (Habilitation BR chargé d'intervention)
  - Tapis d'isolation (au sol)

##### 1ère étape, VAT
- L'AGCP a été désactivé (coupure), puis consigné
- On vérifie à l'aide d'un appareil VAT que le tableau n'est pas sous tension: tension nulle entre neutre et phase(s), entre phase(s) et terre, entre neutre et terre
- Dès lors qu'on a établi que le tableau n'est pas sous tension, on peut enlever les équipements de protection

##### 2ème étape Mesures de résistance
- L'appareil qui lit la résistance (mesurée en $\Omega$ Ohms) fait entendre un bip si la résistance ne dépasse 40 Ohms (à vérifier selon les modèles), mais il faut en tous les cas pouvoir lire la valeur sur l'écran digital de l'appareil

"Il est impératif de vérifier la continuité des conducteurs de protection et des liaisons équipotentielles supplémentaires et principales éventuelles. Elles doivent être testées avec un ohmétre et leur continuité doit être inférieure ou égale à 2 ohms."

([tiré du site web Zoom Elec](https://www.schema-electrique.net/mise-a-la-terre-installation-electrique-norme-NF-C-15-100.html)) 

##### 4ème étape Vérification de l'isolement

(On voit la 3ème étape en suivant)

- Mesure de la qualité de l'isolation des conducteurs (en $\Omega$ Ohms aussi)
- On doit pouvoir mesurer des résistaces dans le domaine des Mega Ohms (milliers de $\Omega$), avec un appareil, le *méga-ohmètre*
- On injecte dans un réseau 230V, une tension de 500V, dans une installation 500V on injectera une tension de 1000V
- Pour une très basse tension, on utilisera une tension de 250V
- L'usage de l'appareil ne nécessite pas l'utilisation des EPI
  - L'appareil n'est pas relié au réseau
  - Il n'injecte un courant électrique que de 1mmA (or le seuil de non lâcher est de 10mmA).

|  Tension nominale du circuit | Tension d'essai  | Résistance minimale d'isolement  |
|---|---|---|
|  Inférieur à 50 V |  250 VDC |  0,25 M $\Omega$ |
| De 50 V à 500 V  |  500 VDC |  0,50 M $\Omega$ |

Pour tester l'isolement, on pourrait tester individuellement chacun des départs de circuit (et on doit observer pour chacun  une résistance d'au moins 0,5M $\Omega$).

On va plutôt considérer l'ensemble des circuits, tous à la fois -- qui sont alors en parallèle. [On se rappelle que la résistance d'un circuit parallèle est plus petite que la résistance la plus faible des circuits qui sont connectés en parallèle.](../1ere_partie/CAP_Elec_1_03.md)

- Ainsi, si la résistance mesurée est au moins égale à 0,5M $\Omega$, c'est qu'elle est au moins égale à cette valeur pour chacun des circuits.

Cette vérification se fait en s'assurant d'abord que tous les circuits sont fermés (tous les disjoncteurs sont "en marche forcée").

##### 3ème étape Vérification d'absence de court-circuit

Avec le test décrit à la section précédente, on ne vérifie pas l'isolement entre phase et neutre.

Pour mesurer la résistance entre phase et neutre, on pourrait procéder circuit par circuit.

- Cependant, s'il y a continuité entre phase et neutre, le multi-mètre indiquera la résistance des appareils alimentés par ce circuit, si par exemple ils sont en marche (ampoule, chauffe-eau, etc.).
- Si la résistance
