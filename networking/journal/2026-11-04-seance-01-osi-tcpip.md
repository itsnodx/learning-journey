# Séance 01 — OSI, TCP/IP et premiers diagnostics

**Date :** 4 novembre 2026  
**Sujet :** comprendre ce que les tests réseau prouvent (et ce qu'ils ne prouvent pas)

## Ce que j'ai travaillé

J'ai repris les couches OSI à partir de situations simples entre mon Mac, le Dell et le switch : deux machines dans le même réseau, un câble débranché, deux sous-réseaux sans routeur et un service web inaccessible malgré un `ping` qui fonctionne.

## Ce que je retiens

- Même sous-réseau : les machines peuvent échanger sans passer par un routeur.
- Câble débranché : commencer par vérifier le lien physique.
- Sous-réseaux différents : vérifier les adresses IP, les masques et la route ou passerelle.
- `ping` réussi, site inaccessible : chercher ensuite du côté du service, du port, du pare-feu ou du DNS selon le cas.

Un `ping` répond à une question précise : est-ce que j'obtiens une réponse ICMP ? Il ne garantit pas le fonctionnement de toutes les applications.

## À tester ensuite

Observer une résolution ARP et des échanges ICMP dans Wireshark. Je garderai les commandes et captures lorsque j'aurai fait ce lab.

[Notes réseau](../README.md) · [Glossaire](../glossaire.md)
