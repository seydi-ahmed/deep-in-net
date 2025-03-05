# Modéle OSI:
OSI (Open Systems Interconnection) est un modéle en 7 couches qui explique la circulation des données dans un réseau.
- couche Physique: transmission des données (câbles, ondes etc.)
- couche Liaison de données: communication entre les appareils (switch...)
- couche Réseau: routage des données avec les adresses IP (routeurs...)
- couche Trasnport: gestion des connexions et de la fiabilité (TCP/UDP)
- couche Session: ouverture, gestion et fermeture des sessions de communication
- couche Présentation: chiffrement, compression et format des données (jpeg, mp3 etc.)
- couche Application: interaction avec l'utilisateur (http, ftp etc.)

# RJ-45 cable?
câble utilisé pour les connexions réseau
- câble droit: relie les appareils de type différent
- câble croisé: relie les appareils de même type

# IP Address:
- suite de 4 nombres séparés par des points. chaque nombre étant compris entre 0 et 255.
- calcul exemple ip: 192.168.1.10 et masque: 255.255.255.0
    - on commence par identifier la partie réseau et la partie hôte
    - les 255 dans le masque représente la partie réseau(192.168.1) et le 0 dans le masque représente la partie hôte (.10)
    - on détermine la plage d'adresse disponible
        - première adresse (adresse réseau): 192.168.1.0 (réservée)
        - derniére adresse (broadcast): 192.168.1.255 (pour envoyer à tout le réseau)
        - adresses disponibles: de 192.168.1.1 à192.168.1.254
- en résumé une adresse réseau est calculée en utilisant le masque de sous-réseau en séparant la partie réseau et la partie appareil. ensuite on attribue les adresses disponibles aux différents appareils.

# What is the function of a switch, how does it operate and what is its role in networking?
- un switch connecte des appareils d'un réseau local
- il apprend les adresses MAC des appareils connectés et envoie les données uniquement au bon destinataire
- il optimise la communication dans le réseau (améliorer la rapidité du réseau, réduit les collisions)

# What is the function of a hub, how does it operate and what is its role in networking?
- tout comme un switch, un hub permet de connecter tous les appareils d'un réseau local moins en intelligent
- il reçoit les données d'un appareil et les distribue à tous les appareils connectés. maintenant c'est aux appareils de vérifier si les données leur sont destinées.
- tout comme un switch mais en plus lent.

# What are the differences between a hub and a switch?
- un switch envoie les données au bon destintaire tandis qu'un hub envoie les données à tous les appareils connectés.

# Can you identify the OSI model layer that the switch and the hub operate on?
- un switch fonctionne à la couche 2 (liaison de données). il utilise les adresses MAC pour envoyer les données au bon appareil.
- un hub fonctionne à la couche 1 (physique). il transmet les signaux sans filtre ni analyse.

# What is a server and what is its purpose in networking?
- un serveur est un systéme qui fournit des services à des appreils appelés client dans un réseau.
- stocker et partager des fichiers, héberger des sites web, gérer des emails etc. fournir des bases de données.

