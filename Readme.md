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

## EX02:
1) What is the function of a switch, how does it operate and what is its role in networking?
- un switch est un appareil qui connecte plusieurs appareils dans un même réseau.
- il apprend les adresses MAC des appareils connectés et envoie les données uniquement aux appareils connectés.
- il améliore la vitesse et l'efficacité du réseau. il permet aux appareils de communiquer directement entre eux.

2) What is the function of a hub, how does it operate and what is its role in networking?
- un hub est aussi un appareil réseau mais plus simple et moins efficace qu'un réseau.
- il reçoit des données d'un appareil connecté et envoie ces données à tous les autres appareils.
- il connecte plusieurs appareils mais sans distinction. il génére beaucoup de trafic et peut créer des collisions de données.

3) What are the differences between a hub and a switch?
```
CRITERE             HUB                             SWITCH
Fonctionnement      Envoie les données à tous       Envoie seulement au bon appareil
Efficacité          Lent (plus de collisions)	    Rapide (évite les collisions)
Gestion du trafic	Pas intelligent                 Gère les adresses MAC
Utilisation	        Petits réseaux                  Réseaux performants
```

4) Can you identify the OSI model layer that the switch and the hub operate on?
- le hub fonctionne à la couche 1 (Physique). il ne fait que transmettre les signaux sans les comprendre
- le switch fonctionne à la couche 2 (Liaison de données). il utilise les adresses MAC pour gérer le trafic et éviter les collisions.

## EX01:
1) What is a server and what is its purpose in networking?
- un serveur est un ordinateur puissant qui fournit des services à d'autres ordinateurs

2) How does DHCP work in a network and what is its function?
- le DHCP attribut automatiquement des adresses ip aux appareils d'un réseau.
- il évite de configurer chaque appareil manuellement.

3) What is the definition of DNS and what role does it play in network communication?
- le DNS traduit un nom de domain en une adresse ip.
- Sans dns il faudrait retenir toutes les adresses ip des sites web.

4) What is the purpose of HTTP and how is it used in networking?
- le http permet de charger des pages web sur un navigateur.
- il utilise le port et fonctionne sans cryptage.

5) What is HTTPS and how does it differ from HTTP?
- c'est la version sécurisée de http.
- plus sécurisée.
- port 443

6) What is the purpose of FTP and how does it operate in network communication?
- permet de tranférer un fichier entre un client et un server.
- connection de commade
- transfert de fichier

7) What is TCP and UDP communication and what distinguishes them from each other?
- ce sont 2 protocoles de communication utilisés pour transmettre des données.
- 📌 TCP
    - connexion fiable (les données arrivent bien)
    - utilisé pour le web, les emails, le ftp.
    - plus lent mais sécurisé
- 📌 UDP
    - pas de vérification, plus rapide que TCP
    - utilisé pour les jeux en ligne, le streaming etc.
    - moins fiable (perte possible de paquets)

8) At which OSI model layer do TCP and UDP operate?
- TCP et UDP fonctionnent à la couche 4 (Transport) du modèle OSI.

9) What is a port in networking and what is its function?
- un port est un numéro qui identifie un numéro spécifique sur un ordinateur. cela permet à plusieurs services de fonctionner sur un même ordinateur.

10) What are the port and OSI model layer for each protocol used?
- port:
    - http(80), https(443), dns(53), ftp(21/21), dhcp(67/68)
- couche:
    - couche 7 (Application)

11) What are the various types of DNS records and what are their purposes?
```
Type d’enregistrement	                Rôle
A	                                    Associe un nom de domaine à une adresse IPv4.
AAAA	                                Associe un nom de domaine à une adresse IPv6.
CNAME	                                Alias d’un autre domaine (ex: www.example.com → example.com).
MX	                                    Indique les serveurs de messagerie (emails).
PTR	                                    Fait l’inverse du A (IP vers nom de domaine).
NS	                                    Indique les serveurs DNS responsables du domaine.
TXT	                                    Stocke des informations diverses (vérification SPF pour les emails).
```