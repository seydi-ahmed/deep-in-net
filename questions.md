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

# 