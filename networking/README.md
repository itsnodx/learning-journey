# Networking

Je reprends les bases des réseaux en parallèle de mes cours et de mes essais sur le Mac, le Dell et les switches. Mes références principales sont Jeremy's IT Lab (CCNA) et Professor Messer (Network+).

Ce README résume ma progression. Mes notes de séance restent dans mon application de notes ; les essais pratiques publiés vont dans [NodX-Lab](https://github.com/itsnodx/NodX-Lab).

## Progression

| Module | Sujet | État |
|---|---|---|
| 01 | Modèles OSI et TCP/IP, premiers diagnostics | En cours |
| 02 | Ethernet, adresses MAC, ARP et switching | À approfondir |
| 03 | IPv4, masques et subnetting | À approfondir |
| 04 | TCP, UDP et services réseau | À approfondir |
| 05 | VLAN, trunks et STP | À approfondir |
| 06 | Routage | À approfondir |
| 07 | Sécurité et dépannage | À approfondir |

Les statuts indiquent ma progression personnelle, pas une validation de compétences.

## Notes — OSI et TCP/IP

Le modèle OSI sépare les communications en sept couches. TCP/IP est la famille de protocoles que j'observe sur les machines.

| Couche OSI | Ce que je regarde |
|---|---|
| 7 — Application | HTTP, DNS, SSH |
| 6 — Présentation | Format et encodage des données |
| 5 — Session | Gestion des sessions |
| 4 — Transport | TCP, UDP, ports |
| 3 — Réseau | IP, passerelle, routage |
| 2 — Liaison | Trames Ethernet, MAC, ARP |
| 1 — Physique | Câbles, ports, liaison |

Ces catégories servent à raisonner : un problème réel ne se résume pas toujours à une seule couche.

**Ce que j'ai retenu des premiers exercices :**
- Deux appareils sur le même réseau peuvent communiquer sans routeur.
- Débrancher le câble casse la liaison physique.
- Pour joindre un autre sous-réseau, il faut une route adaptée.
- Un `ping` réussi ne prouve pas que le serveur web fonctionne.

**Prochain test :** capturer ARP et ICMP avec Wireshark, puis expliquer chaque échange observé.
