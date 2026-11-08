# Glossaire réseau

Définitions courtes, reformulées au fil des séances. Ce glossaire accompagne les [notes réseau](README.md) et le [journal](journal/).

| Terme | Définition |
|---|---|
| **Adresse IP** | Adresse logique utilisée pour identifier une interface et acheminer des paquets dans un réseau IP. |
| **Adresse MAC** | Identifiant de couche liaison utilisé notamment par Ethernet pour livrer une trame sur un réseau local. |
| **ARP** | Protocole IPv4 qui associe une adresse IP locale à une adresse MAC. |
| **Broadcast** | Communication envoyée à tous les hôtes d'un même domaine de diffusion. |
| **CIDR** | Notation d'un préfixe IP, par exemple `192.168.1.0/24`. |
| **DNS** | Service qui résout notamment les noms de domaine en adresses IP. |
| **Ethernet** | Famille de technologies de réseau local définissant notamment les trames et l'accès au support. |
| **ICMP** | Protocole de contrôle et de diagnostic IP, notamment utilisé par `ping`. |
| **Masque de sous-réseau** | Indique quels bits d'une adresse IPv4 appartiennent à la partie réseau. |
| **OSI** | Modèle de référence décrivant les communications en sept couches. |
| **Paquet** | Unité de données de couche réseau (IP). |
| **Passerelle par défaut** | Routeur utilisé lorsqu'une destination se situe hors du réseau directement connecté. |
| **Port TCP/UDP** | Identifiant numérique d'un service ou d'un point de communication de transport. |
| **Routeur** | Équipement qui transfère des paquets IP entre réseaux. |
| **Sous-réseau** | Portion d'un espace d'adressage IP définie par un préfixe. |
| **Switch (commutateur)** | Équipement qui relaie des trames Ethernet, généralement selon les adresses MAC. |
| **TCP** | Protocole de transport orienté connexion avec livraison fiable et ordonnée des octets. |
| **TCP/IP** | Famille de protocoles au cœur des communications Internet. |
| **Trame** | Unité de données de couche liaison, par exemple une trame Ethernet. |
| **UDP** | Protocole de transport sans connexion, qui ne garantit ni la livraison ni l'ordre des datagrammes. |
| **VLAN** | Réseau local virtuel permettant de séparer des domaines de diffusion sur une infrastructure commutée. |
| **Wireshark** | Outil permettant de capturer et d'analyser les paquets et trames réseau. |

## Notes importantes

- Deux machines du même sous-réseau IPv4 peuvent communiquer sans routeur, si la liaison locale et les configurations le permettent.
- Un `ping` réussi prouve une réponse ICMP, **pas** le bon fonctionnement de tous les services applicatifs.
- Pour joindre un autre réseau IP, il faut normalement une route appropriée et une passerelle accessible.

Ce fichier est volontairement évolutif : exemples, corrections et nouveaux termes seront ajoutés après les séances.
