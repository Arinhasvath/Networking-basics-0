# Glossaire des Termes Techniques en Réseau

## OSI (Open Systems Interconnection)
- **Définition** : Modèle conceptuel qui caractérise les fonctions de communication d'un système de télécommunication sans tenir compte de leur structure interne et de leur technologie sous-jacente.
- **Traduction** : Interconnexion des Systèmes Ouverts.
- **Organisation** : Le modèle est organisé en 7 couches, de la plus basse à la plus élevée :
  1. Couche Physique (Physical Layer)
  2. Couche Liaison de Données (Data Link Layer)
  3. Couche Réseau (Network Layer)
  4. Couche Transport (Transport Layer)
  5. Couche Session (Session Layer)
  6. Couche Présentation (Presentation Layer)
  7. Couche Application (Application Layer)

---

## LAN (Local Area Network)
- **Définition** : Réseau connectant des appareils locaux, typiquement dans une petite zone géographique comme un bâtiment ou un campus.
- **Traduction** : Réseau Local.
- **Utilisation Typique** : Interconnexion d’ordinateurs, imprimantes et autres périphériques.

---

## WAN (Wide Area Network)
- **Définition** : Réseau connectant plusieurs LANs sur une grande zone géographique, comme des villes ou des pays.
- **Traduction** : Réseau Étendu.
- **Utilisation Typique** : Internet est l'exemple le plus courant.

---

## Internet
- **Définition** : Réseau mondial qui connecte des millions de réseaux privés, publics, académiques, d’entreprises et gouvernementaux.
- **Traduction** : Internet (pas de traduction directe).

---

## Adresse MAC (Media Access Control)
- **Définition** : Identifiant unique attribué à une interface réseau pour la communication au sein d’un réseau physique.
- **Traduction** : Adresse de Contrôle d’Accès au Média.
- **Utilisation** : Permet d’identifier un appareil au niveau de la couche liaison de données.

---

## Adresse IP (Internet Protocol)
- **Définition** : Numéro attribué à chaque appareil connecté à un réseau pour permettre son identification et sa communication.
- **Traduction** : Adresse de Protocole Internet.
- **Types** :
  - **Adresse Privée** : Utilisée au sein d'un LAN.
  - **Adresse Publique** : Utilisée pour la communication sur Internet.

---

## IPv4 et IPv6
- **IPv4** : Version 4 du protocole Internet, utilise des adresses 32 bits (ex : 192.168.1.1).
- **IPv6** : Version 6, utilise des adresses 128 bits pour répondre à l’épuisement des adresses IPv4.

---

## Localhost
- **Définition** : Nom d’hôte qui fait référence à l’appareil lui-même (adresse IP 127.0.0.1).
- **Traduction** : Boucle Locale.

---

## TCP (Transmission Control Protocol)
- **Définition** : Protocole de transport fiable qui vérifie que les données sont correctement reçues.
- **Traduction** : Protocole de Contrôle de Transmission.
- **Caractéristique** : Transferts lents mais fiables.

---

## UDP (User Datagram Protocol)
- **Définition** : Protocole de transport rapide qui ne garantit pas la livraison des données.
- **Traduction** : Protocole de Datagramme Utilisateur.
- **Caractéristique** : Transferts rapides mais moins fiables.

---

## Ports TCP/UDP
- **Définition** : Points d’entrée ou de sortie d’un appareil réseau pour les communications.
- **Exemples Communs** :
  - Port 22 : SSH
  - Port 80 : HTTP
  - Port 443 : HTTPS

---

## Ping / ICMP (Internet Control Message Protocol)
- **Ping** : Commande qui vérifie la connectivité d'un appareil sur un réseau.
- **ICMP** : Protocole utilisé pour envoyer des messages d’erreur ou des requêtes (par ex. ping).
- **Traduction** : Protocole de Message de Contrôle Internet.

---

## DNS (Domain Name System)
- **Définition** : Système qui traduit les noms de domaine lisibles par l’humain (par ex. www.google.com) en adresses IP compréhensibles par les machines.
- **Traduction** : Système de Noms de Domaine.
- **Utilisation** : Facilite l’accès aux sites Web sans mémoriser des adresses IP complexes.

---

## NAT (Network Address Translation)
- **Définition** : Méthode permettant à plusieurs appareils sur un réseau local (LAN) d'utiliser une seule adresse IP publique pour accéder à Internet.
- **Traduction** : Traduction d’Adresses Réseau.
- **Bénéfices** : Améliore la sécurité et économise les adresses IP.

---

## VPN (Virtual Private Network)
- **Définition** : Technologie qui crée une connexion sécurisée entre un utilisateur et un réseau sur Internet.
- **Traduction** : Réseau Privé Virtuel.
- **Utilisation** : Protection de la vie privée et accès à des contenus géo-restreints.

---

## Proxy
- **Définition** : Serveur intermédiaire qui relaye les requêtes entre un client et un serveur.
- **Traduction** : Proxy (pas de traduction directe).
- **Utilisation** : Anonymisation ou contrôle des accès.

---

## SSH (Secure Shell)
- **Définition** : Protocole qui permet une connexion sécurisée à un ordinateur distant.
- **Traduction** : Shell Sécurisé.
- **Port par Défaut** : 22.

---

## HTTP et HTTPS
- **HTTP** : Protocole de communication pour le transfert de pages Web.
  - **Traduction** : Protocole de Transfert Hypertexte.
  - **Port par Défaut** : 80.
- **HTTPS** : Version sécurisée de HTTP.
  - **Traduction** : Protocole de Transfert Hypertexte Sécurisé.
  - **Port par Défaut** : 443.

---

## FTP (File Transfer Protocol)
- **Définition** : Protocole standard pour le transfert de fichiers entre un client et un serveur sur un réseau.
- **Traduction** : Protocole de Transfert de Fichiers.
- **Ports** :
  - 20 : Transfert de données.
  - 21 : Commandes.

---

## Firewall (Pare-feu)
- **Définition** : Système de sécurité réseau qui surveille et contrôle le trafic réseau entrant et sortant.
- **Traduction** : Pare-feu.
- **Utilisation** : Protection contre les accès non autorisés.

---

## VLAN (Virtual Local Area Network)
- **Définition** : Technique permettant de segmenter un réseau physique en réseaux logiques distincts.
- **Traduction** : Réseau Local Virtuel.
- **Avantage** : Améliore la sécurité et la gestion des réseaux.

---

## Load Balancer
- **Définition** : Dispositif qui répartit le trafic réseau ou applicatif entre plusieurs serveurs.
- **Traduction** : Répartiteur de Charge.
- **Utilisation** : Optimisation des performances et tolérance aux pannes.

---

## QoS (Quality of Service)
- **Définition** : Ensemble de technologies permettant de gérer la priorité des données sur un réseau.
- **Traduction** : Qualité de Service.
- **Exemple** : Priorisation de la voix sur IP (VoIP) par rapport au téléchargement de fichiers.

---

## DHCP (Dynamic Host Configuration Protocol)
- **Définition** : Protocole qui attribue automatiquement des adresses IP aux appareils d’un réseau.
- **Traduction** : Protocole de Configuration Dynamique des Hôtes.
- **Utilisation** : Réduit la complexité de la gestion des adresses IP.
