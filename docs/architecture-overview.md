# Vue d'architecture — version publiable

## Objectif

L'architecture répond aux besoins d'une entreprise industrielle manipulant des données clients, des plans de conception et des données de production. La confidentialité et l'intégrité des fichiers d'ingénierie sont donc aussi importantes que la disponibilité des outils métiers.

## Principes directeurs

### Défense en profondeur

Deux niveaux de filtrage séparent Internet, la zone exposée et les réseaux internes. Un compromis d'un service exposé ne doit pas donner directement accès aux services métier ou aux postes utilisateurs.

### Segmentation par exposition et par métier

L'architecture sépare au minimum :

- les services exposés dans une DMZ ;
- l'identité et la PKI ;
- les serveurs métiers ;
- l'administration ;
- les postes bureautiques ;
- l'ingénierie et les outils CAO ;
- la production ;
- la sauvegarde et la supervision.

Chaque communication inter-zone est autorisée uniquement lorsqu'elle répond à un besoin identifié. La politique cible est un refus par défaut, complété par des flux explicitement justifiés.

### Identité centralisée et chiffrement

L'architecture prévoit une identité centralisée, des groupes de sécurité, des stratégies de poste et une PKI à plusieurs niveaux. Les services utilisent des canaux chiffrés et l'accès distant repose sur une authentification forte.

### Observation et résilience

Les journaux des composants critiques sont centralisés pour faciliter la détection et l'investigation. Les sauvegardes, le versioning des fichiers et la séparation des environnements participent à la reprise après incident.

## Composants présentés à haut niveau

| Domaine | Rôle de sécurité |
| --- | --- |
| Pare-feu périmétrique | Filtrage Internet, contrôle de l'exposition, NAT et protection de la DMZ. |
| Pare-feu interne | Filtrage inter-zones et limitation des mouvements latéraux. |
| DNS et domaine | Résolution maîtrisée, séparation logique des usages et socle d'identité. |
| Reverse proxy | Point d'entrée contrôlé pour les services web publiés. |
| Proxy sortant | Maîtrise des flux web sortants et traçabilité. |
| Identité / PKI | Authentification, autorisation, groupes et certificats. |
| SIEM et détection | Centralisation des événements, corrélation et alertes. |
| Sauvegarde | Récupération, restauration et réduction de l'impact ransomware. |

## Ce qui reste privé

Les documents de conception internes contiennent des informations qui ne doivent pas être publiées dans un portfolio : plan d'adressage, inventaire détaillé, noms d'hôtes, matrice de flux complète, règles de filtrage, configurations VPN, certificats, comptes et procédures opérationnelles détaillées.
