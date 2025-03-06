# Deep-In-Net

Ce fichier README.md contient une clarification des connaissances acquises et des étapes suivies pour recréer l'architecture réseau dans Cisco Packet Tracer.

## Connaissances Acquises

1. **Configuration des Routeurs :**
   - J'ai appris à configurer les routeurs en utilisant l'interface de ligne de commande (CLI) de Cisco.
   - Configuration des interfaces avec des adresses IP.
   - Configuration des routes statiques pour permettre la communication entre les différents sous-réseaux.

2. **Configuration des PC et Laptops :**
   - Attribution d'adresses IP statiques ou configuration pour obtenir une adresse IP via DHCP.
   - Vérification de la connectivité avec des commandes comme `ping` ou directement via le logo de message.

3. **Test et Validation :**
   - Utilisation de `ping` pour vérifier la connectivité entre les différents périphériques.

## Étapes pour Recréer l'Architecture Réseau
1) configuration de chaque réseau 
- placement: placer les pc, switch, routeurs et éventuellement les serveurs
- distribution des adresses ip:
   - trouver l'adresse réseau et le masque pour chaque réseau puis calculer la plage d'adresse disponibles
   - donner aux appreils des ip qui sont dans la plage
2) configuration des routeurs pour les réseaux locaux
- aller dans le routeur
- dans config/interface/fastethernet(ou le câble utilisé) mettre le gateway du réseau
3) configuration entre les routeurs
- même principe
- allez dans chaque routeur
- dans Se2/0 (où le câble correspondant) mettre le gateway réseau choisi
4) configuration entre les machines de différents réseaux (avec OSPF ou RIP)
- OSPF: sur chaque routeur:
   - enable
   - configure terminal
   - router OSPF 1
   - network + ```adresse réseau à laquelle il(le routeur) appartient``` + ```l'inverse du mask(mettre des 0 à la place des 1 et des 1 à la place des 0) ``` + are 0 + Enttrée
- RIP: sur chaque routeur:
   - aller dans config/routing/rip
   - mettre l'adresse réseau(où les adresses) à la quelle le routeur apparatient
5) commencer la simulation

## Conclusion

À travers cet exercice, j'ai acquis une compréhension approfondie de la configuration des routeurs, switches, et périphériques finaux dans Cisco Packet Tracer. J'ai également appris à planifier et à tester un réseau complexe, en m'assurant que tous les éléments fonctionnent correctement ensemble.

## Développeur:
- Prénom NOM: Mouhamed DIOUF
- Email: Diouf.mouhamed3@ugb.edu.sn

## Calcul en ligne:
- https://cric.grenoble.cnrs.fr/Administrateurs/Outils/CalculMasque/