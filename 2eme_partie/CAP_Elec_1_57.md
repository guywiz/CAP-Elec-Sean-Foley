# CAP Elec 1.57 Alim bâtiment secondaire
## Foley Services Elec - [Programme 2ème partie](../2eme_partie/README.md)

### 1.57 Alim bâtiment secondaire

- **Accès à la vidéo** [1.57 Alim bâtiment secondaire](https://youtu.be/kEPQB54pdL4)

Alimentation d'un bâtiment secondaire (atelier, garage, studio, ...) à partir de l'alimentation d'une habitation principale

- Quelle gaine pour acheminer l'alimentation jusqu'au bâtiment secondaire
- Bilan des appareils qui seront alimentés/utilisés dans ce bâtiment
  - Calcul de l'intensité requise

  
A des fins d'illustration, imaginons que le bilan nous amène à évaluer l'intensité requise à 30A.

- Un câble gainé passera dans une tranchée jusqu'au bâtiment
- Un disjoncteur 32A (> 30A) qui protégera le câble alimnetant le bâtiment secondaire
- On peut être tenté de conclure à l'utilisation d'un câble de section 6mm2 (qui correspond au disjoncteur 32A)
  - Mais la longueur $L$ du câble peut induire une chute de tension ... à calculer -- voir [la leçon sur la chute de tension](./CAP_Elec_1_46.md)

#### Tranchée

- Profondeur 50cm minimum, si passage de voiture il faut aller à 80cm
- Gaine TPC (rouge) pour l'alimentation
  - Pourquoi ne pas aussi inclure une gaine (verte) pour éventuelllement passer des câbles com
- Recouvrir les gaines avec du sable d'abord, pour éviter de compresser les gaines (avec des caillous) sur une hauteur de 30cm
  - Avant de recouvrir d'un filet avertisseur (rouge - courant fort, vert - courant faible) 
  - On utilise un câble R2V prévu pour tenir les conditions changeantes et aléas mécaniques

- Le disjoncteur 32A protégeant le câble ***ne doit pas*** être ajouté aux disjoncteurs associés à un interrupteur différentiel du tableau existant
  - Le câble sera acheminé à un interrupterur différentiel dans un tableau indépendant

#### Protecttion équipotentielle (terre)

- La câble R2V doit acheminer une liaison de terre
  - Même si on aménage un second piquet de terre, ce câble doit comporter une fil PE, le second piquet de terre n'épargne pas d'avoir à acheminer une liaison PE au niveau du câble
- En effet, même si un second piquet de terre était installé pour protéger le tableau secondaire
  - Si la liaison à la terre par le câble était inexistante, des appareils pourraient connaître une différence de potentiel (non nulle) parce que branché électriquement au tableau secondaire et liés aux liaisons équipotentielles secondaire (réseau d'eau, avec l'exemple du karcher)