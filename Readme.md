# Deep-In-Net

## EX01:
1) Câble RJ-45:
- Un câble RJ-45 est un câble utilisé principalement pour les connexions Ethernet. il utilise une fiche à 8 broches (8P8C - 8 positions, 8 contacts) et transporte des signaux de données dans des appareils comme l'ordinateur par exemple.
2) Différence entre un câble RJ-45 direct et un câblr RJ-45 croisé:
- Câble direct(straight-through): il connecte les mêmes broches de chaque côté (ex. : broche 1 → broche 1, broche 2 → broche 2, etc.). il utilisé pour relier les périphériques de types différents (PC ↔ Switch, Switch ↔ Routeur).
- Câble croisé(crossover): Certaines paires de fils sont inversées (ex. : broche 1 ↔ broche 3, broche 2 ↔ broche 6). il est utilisé pour relier les périphériques de même type (PC ↔ PC, Switch ↔ Switch). 
3) Comment sont calculés les adresses IP?
- Une adresse IP (Ipv4) est composée de 32 bits généralement divisée en 4 octets (ex: 192.168.1.1). son calcul dépend du masque de sous-réseau.
- Adresse réseau: c'est l'adresse IP avec la partie hôte remplacée par des zéros (192.168.1.0/24).
- Adresse de diffusion: c'est l'adresse IP avec la partie hôte remplacée par des 1 (192.168.1.255/24).
- Plage d'adresse utilisable: entre l'adresse réseau et l'adresse de diffusion (192.168.1.0 à 192.168.1.254 pour un /24).
- Pour un IPv6 le principe est le même mais les adresses sont sur 128 bits.