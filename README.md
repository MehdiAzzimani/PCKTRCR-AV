# Réseau d'un cabinet d'avocats — Cisco Packet Tracer

Maquette de l'infrastructure réseau d'un cabinet d'avocats : postes répartis par service, serveur assurant DHCP et DNS, imprimante réseau et accès Internet.

Exercice réalisé sous Cisco Packet Tracer dans le cadre de ma formation.

## Architecture

| Élément | Détail |
| --- | --- |
| Adressage | IPv4, `192.168.1.0/24` |
| Commutation | Tous les équipements raccordés à un switch central (`Switch0`) |
| Accès Internet | Routeur sans fil WRT300N |
| Serveur | HP Proliant ML30 Gen10 — rôles DHCP et DNS |
| Postes | Répartis par service : Avocats, Secrétariat, Comptabilité, Direction |
| Périphérique | 1 imprimante réseau sur le switch |

## Services configurés

### DHCP

Le serveur distribue les adresses automatiquement sur la plage `192.168.1.2` à `192.168.1.151`.

### DNS

Le même serveur assure la résolution des noms internes pour les postes clients.

### Sécurisation des équipements

Le routeur et le switch central sont protégés par mots de passe : mot de passe d'activation (mode privilégié) et compte administrateur distinct sur chacun.

## Contenu du dépôt

| Fichier | Description |
| --- | --- |
| `ReseauAv.pkt` | Maquette à ouvrir dans Cisco Packet Tracer |

## Compétences mises en œuvre

Adressage IPv4 et sous-réseaux · configuration DHCP et DNS · commutation · sécurisation des accès aux équipements Cisco
