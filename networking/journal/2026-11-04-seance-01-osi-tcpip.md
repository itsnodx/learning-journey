# Séance 01 — Modèles OSI/TCP-IP et diagnostic de connectivité

**Date :** 2026-11-04  
**Module :** 01 — Fondamentaux des réseaux  
**Sujet :** communication locale, couches OSI, rôle de la passerelle

## Objectif

Relier les couches des modèles OSI et TCP/IP à des situations simples de diagnostic réseau, avant d'observer les paquets avec Wireshark.

## Concepts travaillés

- **Couche 1 — Physique :** un câble Ethernet débranché empêche la transmission sur le lien concerné.
- **Couche 2 — Liaison :** un switch Ethernet peut acheminer des trames entre appareils d'un même réseau local.
- **Couche 3 — Réseau :** une destination hors du sous-réseau nécessite une route appropriée, généralement via une passerelle.
- **Couches supérieures :** un `ping` fonctionnel ne garantit pas qu'un serveur web ou la résolution DNS fonctionne.

## Scénarios discutés et observations rapportées

| Scénario | Résultat / interprétation |
|---|---|
| Mac et Dell connectés au même réseau local via un switch | Un échange ICMP est possible sans routeur intermédiaire. |
| Câble Ethernet débranché | Première piste : défaut de connectivité physique (couche 1). |
| Machines sur des sous-réseaux différents, sans routeur configuré | La communication IP inter-réseaux échoue en l'absence de route adaptée. |
| `ping` vers le Dell possible, mais accès web impossible | Il faut examiner le service web, le port, le pare-feu et, si un nom est utilisé, DNS ; le seul `ping` ne localise pas définitivement la panne. |

Ces notes synthétisent les exercices et raisonnements de la séance ; elles ne constituent pas encore une capture Wireshark ni un compte rendu de laboratoire complet.

## Ce que je retiens

Une communication se diagnostique en isolant les fonctions : lien physique, réseau local, adressage et routage IP, transport, puis service applicatif. Chaque test apporte une preuve limitée.

## À approfondir

- Observer une résolution ARP et un échange ICMP dans Wireshark.
- Comparer trafic local et trafic destiné à une passerelle.
- Relever les commandes exactes, adresses de test et captures **après réalisation** du laboratoire.

## Liens

- [Notes du module](../README.md)
- [Glossaire](../glossaire.md)
- [NodX-Lab](https://github.com/itsnodx/NodX-Lab)
