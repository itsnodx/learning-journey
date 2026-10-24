
# Networking

Ce dossier rassemble mes notes sur les réseaux informatiques, des notions fondamentales jusqu'aux technologies utilisées dans les réseaux d'entreprise.

Je m'appuie notamment sur les cours de Jeremy's IT Lab (CCNA) et de Professor Messer (Network+), en complément de mes cours universitaires.

Les expérimentations réalisées sur mes équipements physiques sont documentées dans [NodX-Lab](https://github.com/itsnodx/NodX-Lab).

## Progression

| Module | Sujet | État |
|---|---|---|
| 01 | Fondamentaux des réseaux et modèles OSI/TCP-IP |
| 02 | Ethernet, adresses MAC et commutation  |
| 03 | IPv4, masques et subnetting |
| 04 | TCP, UDP et protocoles applicatifs |
| 05 | VLAN, trunks et STP |
| 06 | Routage et interconnexion des réseaux |
| 07 | Sécurité et dépannage réseau |

Ce tableau présente l'organisation de mon apprentissage personnel. Certains sujets ont déjà été abordés pendant mes cours universitaires et seront approfondis progressivement.

## Notes — Modèles OSI et TCP/IP

Le modèle OSI décrit les communications réseau en sept couches. Le modèle TCP/IP représente plus directement l'architecture utilisée sur les réseaux actuels.

Voici quelques exemples de technologies et d'équipements associés aux couches OSI :

| Couche OSI | Exemples |
|---|---|
| 7 — Application | HTTP, DNS, SSH |
| 6 — Présentation | Encodage et représentation des données |
| 5 — Session | Gestion des sessions de communication |
| 4 — Transport | TCP, UDP |
| 3 — Réseau | IPv4, IPv6, routage, Cisco 3750-X |
| 2 — Liaison de données | Ethernet, adresses MAC, switches Cisco et TP-Link |
| 1 — Physique | Câbles Cat6, connecteurs et signaux |

Ces couches sont un modèle conceptuel : dans la pratique, certaines technologies remplissent plusieurs fonctions.

Le TP-Link TL-SG1016DE et le Cisco 2960-X assurent principalement la commutation Ethernet de couche 2. Le Cisco 3750-X permettra également d'étudier les fonctions de routage de couche 3.

## Prochaines expérimentations

Observer les échanges entre plusieurs machines avec Wireshark, notamment les trames Ethernet, ARP, ICMP et les communications TCP/IP.
