# Networking-basics #0

# Curriculum [C#24] Fondations v2 - Partie 3

Moyenne : 12,27%

## Badge de projet

Bases du réseau #0

**Novice**

Par : Sylvain Kalache
Poids : 1

Votre score sera mis à jour au fur et à mesure de votre progression.

## Description

### Ressources

Lire ou regarder :

- Modèle OSI
- Différents types de réseaux
- Réseau LAN
- Réseau WAN
- Internet
- Adresse MAC
- Qu'est-ce qu'une adresse IP
- Adresse privée et publique
- IPv4 et IPv6
- Localhost
- TCP et UDP
- Ports TCP/UDP
- Liste
- Qu'est-ce que le ping /ICMP
- Paramètres positionnels

man ou help :
- netstat
- ping

## Objectifs d'apprentissage

À la fin de ce projet, vous devriez être capable d'expliquer à n'importe qui, sans l'aide de Google :

### Modèle OSI
- Ce que c'est
- Combien de couches il comporte
- Comment il est organisé

### Qu'est-ce qu'un LAN
- Utilisation typique
- Taille géographique typique

### Qu'est-ce qu'un WAN
- Utilisation typique
- Taille géographique typique

### Qu'est-ce qu'Internet
- Qu'est-ce qu'une adresse IP
- Quels sont les 2 types d'adresse IP
- Qu'est-ce que localhost
- Qu'est-ce qu'un sous-réseau
- Pourquoi IPv6 a été créé

### TCP/UDP
- Quels sont les 2 protocoles de transfert de données principalement utilisés pour IP (niveau de transfert sur le schéma OSI)
- Quelle est la principale différence entre TCP et UDP
- Qu'est-ce qu'un port
- Mémoriser les numéros de port pour SSH, HTTP et HTTPS
- Quel outil/protocole est souvent utilisé pour vérifier si un appareil est connecté à un réseau

## Exigences

### Général
- Éditeurs autorisés : vi, vim, emacs
- Tous vos fichiers de script Bash seront interprétés sur Ubuntu 20.04 LTS
- Tous vos fichiers doivent se terminer par une nouvelle ligne
- Un fichier README.md, à la racine du dossier du projet, est obligatoire
- Tous vos fichiers de script Bash doivent être exécutables
- Votre script Bash doit passer shellcheck sans aucune erreur
- La première ligne de tous vos scripts Bash doit être exactement #!/usr/bin/env bash
- La deuxième ligne de tous vos scripts Bash doit être un commentaire expliquant ce que fait le script

## Plus d'informations

La deuxième ligne de tous vos scripts Bash doit être un commentaire expliquant ce que fait le script

Pour les tâches de type questions à choix multiples, tapez simplement le numéro de la bonne réponse dans votre fichier de réponse, ajoutez une nouvelle ligne pour chaque nouvelle réponse, exemple :

Quelle est la position la plus importante dans une entreprise de logiciels ?
1. Chef de projet
2. Développeur backend
3. Administrateur système

```
sylvain@ubuntu$ cat foo_answer_file
3
sylvain@ubuntu$
```

Source pour la question 1 ici

## Tâches

### 0. Modèle OSI
obligatoire

OSI (Open Systems Interconnection) est un modèle abstrait pour décrire la communication en couches et la conception de réseau informatique. L'idée est de séparer les différentes parties de ce qui rend la communication possible. Il est organisé du niveau le plus bas au niveau le plus élevé :

Le niveau le plus bas : couche 1 qui est pour la transmission sur les couches physiques avec impulsion électrique, signal lumineux ou radio
Le niveau le plus élevé : couche 7 qui est pour la communication spécifique à l'application comme SNMP pour les emails, HTTP pour votre navigateur web, etc
Gardez à l'esprit que le modèle OSI est un concept, ce n'est même pas tangible. Le modèle OSI n'effectue aucune fonction dans le processus de mise en réseau. C'est un cadre conceptuel pour que nous puissions mieux comprendre les interactions complexes qui se produisent. La plupart des fonctionnalités du modèle OSI existent dans tous les systèmes de communication.

Dans ce projet, nous nous concentrerons principalement sur :

- La couche Transport et en particulier TCP/UDP
- Sur la couche Réseau avec IP et ICMP

L'image ci-dessous décrit plus concrètement comment vous pouvez vous rapporter à chaque niveau.

Questions :

Qu'est-ce que le modèle OSI ?
1. Ensemble de spécifications que les fabricants de matériel réseau doivent respecter
2. Le modèle OSI est un modèle conceptuel qui caractérise les fonctions de communication d'un système de télécommunication sans tenir compte de leur structure interne et de leur technologie sous-jacentes
3. Le modèle OSI est un modèle qui caractérise les fonctions de communication d'un système de télécommunication en tenant fortement compte de leur structure interne et de leur technologie

Comment le modèle OSI est-il organisé ?
1. Alphabétiquement
2. Du niveau le plus bas au niveau le plus élevé
3. Au hasard

Repo :
- Dépôt GitHub : holbertonschool-network
- Répertoire : basics_0
- Fichier : 0-OSI_model

0/2 pts

### 1. Types de réseau
obligatoire

LAN connecte les appareils locaux ensemble, WAN connecte les LAN ensemble, et les WAN fonctionnent sur Internet.

Questions :

À quel type de réseau un ordinateur en local est-il connecté ?
1. Internet
2. WAN
3. LAN

Quel type de réseau pourrait connecter un bureau dans un bâtiment à un autre bureau dans un bâtiment à quelques rues de là ?
1. Internet
2. WAN
3. LAN

Quel réseau utilisez-vous lorsque vous naviguez sur www.google.com depuis votre smartphone (non connecté au Wifi) ?
1. Internet
2. WAN
3. LAN

Repo :
- Dépôt GitHub : holbertonschool-network
- Répertoire : basics_0
- Fichier : 1-types_of_network

0/3 pts

### 2. Adresse MAC et IP
obligatoire

Questions :

Qu'est-ce qu'une adresse MAC ?
1. Le nom d'une interface réseau
2. L'identifiant unique d'une interface réseau
3. Une interface réseau

Qu'est-ce qu'une adresse IP ?
1. Est aux appareils connectés à un réseau ce que l'adresse postale est aux maisons
2. L'identifiant unique d'une interface réseau
3. Est un nombre que les appareils réseau utilisent pour se connecter aux réseaux

Repo :
- Dépôt GitHub : holbertonschool-network
- Répertoire : basics_0
- Fichier : 2-MAC_and_IP_address

0/2 pts

### 3. UDP et TCP
obligatoire

Remplissons les parties vides dans le dessin ci-dessus.

Questions :

Quelle affirmation est correcte pour la boîte TCP :
1. C'est un protocole qui transfère des données de manière lente mais sûre
2. C'est un protocole qui transfère des données rapidement mais pourrait perdre des données en cours de route

Quelle affirmation est correcte pour la boîte UDP :
1. C'est un protocole qui transfère des données de manière lente mais sûre
2. C'est un protocole qui transfère des données rapidement mais pourrait perdre des données en cours de route

Quelle affirmation est correcte pour le travailleur TCP :
1. Avez-vous reçu les boîtes x, y, z ?
2. Puis-je augmenter le rythme auquel je vous envoie des boîtes ?

Repo :
- Dépôt GitHub : holbertonschool-network
- Répertoire : basics_0
- Fichier : 3-UDP_and_TCP

0/3 pts

### 4. Ports TCP et UDP
obligatoire

Une fois que les paquets ont été envoyés au bon appareil réseau en utilisant IP en utilisant soit UDP soit TCP comme mode de transport, ils doivent effectivement entrer dans l'appareil réseau. Si nous continuons la comparaison d'un appareil réseau avec votre maison, où l'adresse IP est comme votre adresse postale, les ports UDP et TCP sont comme les fenêtres et les portes de votre lieu.

Un appareil réseau TCP/UDP a 65535 ports. Certains d'entre eux sont officiellement réservés pour un usage spécifique, certains sont connus pour être utilisés pour un usage spécifique (mais rien n'est officiellement déclaré) et le reste est libre d'utilisation.

Bien que la liste complète des ports ne doive pas être mémorisée, il est important de connaître les ports les plus utilisés, commençons par en retenir 3 :

- 22 pour SSH
- 80 pour HTTP
- 443 pour HTTPS

Notez qu'une IP spécifique + port = socket.

Écrivez un script Bash qui affiche les ports d'écoute :

- Qui ne montre que les sockets d'écoute
- Qui montre le PID et le nom du programme auquel chaque socket appartient

Exemple :

```bash
sylvain@ubuntu$ sudo ./4-TCP_and_UDP_ports
Active Internet connections (only servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State       PID/Program name
tcp        0      0 *:sunrpc                *:*                     LISTEN      518/rpcbind
tcp        0      0 *:ssh                   *:*                     LISTEN      1240/sshd
tcp        0      0 *:32938                 *:*                     LISTEN      547/rpc.statd
tcp6       0      0 [::]:sunrpc             [::]:*                  LISTEN      518/rpcbind
tcp6       0      0 [::]:ssh                [::]:*                  LISTEN      1240/sshd
tcp6       0      0 [::]:33737              [::]:*                  LISTEN      547/rpc.statd
udp        0      0 *:sunrpc                *:*                                 518/rpcbind
udp        0      0 *:691                   *:*                                 518/rpcbind
udp        0      0 localhost:723           *:*                                 547/rpc.statd
udp        0      0 *:60129                 *:*                                 547/rpc.statd
udp        0      0 *:3845                  *:*                                 562/dhclient
udp        0      0 *:bootpc                *:*                                 562/dhclient
udp6       0      0 [::]:47444              [::]:*                              547/rpc.statd
udp6       0      0 [::]:sunrpc             [::]:*                              518/rpcbind
udp6       0      0 [::]:50038              [::]:*                              562/dhclient
udp6       0      0 [::]:691                [::]:*                              518/rpcbind
Active UNIX domain sockets (only servers)
Proto RefCnt Flags       Type       State         I-Node   PID/Program name    Path
unix  2      [ ACC ]     STREAM     LISTENING     7724     518/rpcbind         /run/rpcbind.sock
unix  2      [ ACC ]     STREAM     LISTENING     6525     1/init              @/com/ubuntu/upstart
unix  2      [ ACC ]     STREAM     LISTENING     8559     835/dbus-daemon     /var/run/dbus/system_bus_socket
unix  2      [ ACC ]     STREAM     LISTENING     9190     1087/acpid          /var/run/acpid.socket
unix  2      [ ACC ]     SEQPACKET  LISTENING     7156     378/systemd-udevd   /run/udev/control
sylvain@ubuntu$
```

Repo :
- Dépôt GitHub : holbertonschool-network
- Répertoire : basics_0
- Fichier : 4-TCP_and_UDP_ports

0/1 pt

### 5. L'hôte est-il sur le réseau
obligatoire

Le protocole ICMP (Internet Control Message Protocol) est un protocole de la suite de protocoles Internet. Il est utilisé par les appareils réseau, pour vérifier si d'autres appareils réseau sont disponibles sur le réseau. La commande ping utilise ICMP pour s'assurer qu'un appareil réseau reste en ligne ou pour résoudre des problèmes sur le réseau.

Écrivez un script Bash qui ping une adresse IP passée en argument.

Exigences :

- Accepte une chaîne comme argument
- Affiche Usage: 5-is_the_host_on_the_network {IP_ADDRESS} si aucun argument n'est passé
- Ping l'IP 5 fois

Exemple :

```bash
sylvain@ubuntu$ ./5-is_the_host_on_the_network 8.8.8.8
PING 8.8.8.8 (8.8.8.8) 56(84) bytes of data.
64 bytes from 8.8.8.8: icmp_seq=1 ttl=63 time=12.9 ms
64 bytes from 8.8.8.8: icmp_seq=2 ttl=63 time=13.6 ms
64 bytes from 8.8.8.8: icmp_seq=3 ttl=63 time=7.83 ms
64 bytes from 8.8.8.8: icmp_seq=4 ttl=63 time=11.3 ms
64 bytes from 8.8.8.8: icmp_seq=5 ttl=63 time=7.57 ms

--- 8.8.8.8 ping statistics ---
5 packets transmitted, 5 received, 0% packet loss, time 4006ms
rtt min/avg/max/mdev = 7.570/10.682/13.679/2.546 ms
sylvain@ubuntu$
sylvain@ubuntu$ ./5-is_the_host_on_the_network
Usage: 5-is_the_host_on_the_network {IP_ADDRESS}
sylvain@ubuntu$
```

Il est intéressant de regarder la valeur de temps, qui est le temps qu'il a fallu pour que la requête ICMP aille à l'IP 8.8.8.8 et revienne à mon hôte. L'IP 8.8.8.8 appartient à Google, et le trajet aller-retour le plus rapide entre mon ordinateur et Google était de 7,57 ms, ce qui est assez rapide, ce qui est un signe que le chemin réseau entre mon ordinateur et le centre de données de Google est en bon état.

Citations:
[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/29334386/eb50ae0c-c3d0-4fc3-b69c-841575b9fb5f/paste.txt
