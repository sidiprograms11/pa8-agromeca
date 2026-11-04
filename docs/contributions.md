# Contributions et responsabilité RACI

## Contribution de Sidi Oumar GANO

La matrice RACI du projet et le suivi des livrables attribuent les responsabilités suivantes à Sidi :

| Périmètre | Rôle | Preuve de contribution |
| --- | --- | --- |
| Dossier d'Architecture Technique | Auteur principal | Rédaction complète du DAT, de la création à la version finale ; architecture, zones de sécurité, services, exploitation, continuité et matrice de flux. |
| Pare-feu périmétrique | Responsable / approbateur, en co-responsabilité | Conception du filtrage périmétrique et de l'organisation des zones exposées. |
| Pare-feu interne | Responsable / approbateur, en co-responsabilité | Contrôle inter-zones et principe du moindre privilège. |
| Règles inter-VLAN | Approbateur | Validation de la cohérence des flux entre zones. |
| DNS master / slave et resolvers | Responsable / approbateur | Conception de l'architecture DNS et de la séparation des rôles. |
| Domaine | Responsable / approbateur | Configuration et cohérence du périmètre de domaine. |
| Reverse proxy | Responsable / approbateur | Publication maîtrisée des services web. |
| Proxy sortant | Responsable / approbateur | Maîtrise des flux web sortants. |
| Schéma d'architecture | Co-auteur | Construction de la vue globale avec les membres désignés. |
| Analyse de risques | Contributeur | Contribution en soutien de l'auteure principale. |

## Contribution de Ezekiel BOUNDA DJIKUI

La matrice RACI du projet et l'inventaire des machines virtuelles attribuent les responsabilités suivantes à Ezekiel :

| Périmètre | Rôle | Preuve de contribution |
| --- | --- | --- |
| Nextcloud | Responsable / approbateur (R/A) | Déploiement et configuration de la plateforme de stockage et de collaboration ; machines virtuelles `EZK-Nextcloud` et `EZK-Nextcloud-Collab`. |
| Dolibarr (ERP/CRM) | Responsable / approbateur (R/A) | Mise en place de la solution de gestion d'entreprise sur un environnement Linux Debian ; machine virtuelle `EZK-Dolibarr`. |
| Extranet Fedora | Responsable / approbateur (R/A) | Déploiement et configuration de l'environnement extranet de l'entreprise, hébergé sur Fedora. |
| MariaDB | Responsable / approbateur (R/A) | Installation et configuration des serveurs de bases de données destinés aux services applicatifs, notamment `EZK-MariaDB` et `EZK-MariaDB-Extranet`. |
| Intégration réseau et sécurité | Consulté | Participation aux échanges techniques concernant la segmentation VLAN, les pare-feu, la gestion des accès, les certificats SSL/TLS et l'intégration des services applicatifs. |
| Supervision et sauvegardes | Consulté | Participation aux échanges concernant la supervision Splunk et la stratégie de sauvegarde Bacula. |
| Rapport d'éco-conception | Co-auteur | Contribution à la rédaction du rapport `ecoConception_AgroMeca.pdf` avec Lamyae, portant sur l'optimisation et l'impact environnemental de l'infrastructure informatique. |

Les mentions « en co-responsabilité » et « contributeur » sont volontaires : le projet était collectif et ce portfolio n'attribue pas le travail des autres membres à une seule personne.

## Contribution de Yann

Yann ([@yann401](https://github.com/yann401)) a assuré la prise en charge de l'ensemble des services de messagerie du projet PA8 — AgroMeca, notamment la configuration SMTP et l'intégration du courrier électronique dans l'infrastructure.

| Périmètre | Rôle | Contribution |
| --- | --- | --- |
| Services de messagerie | Responsable du périmètre | Mise en place et configuration des services de courrier électronique du projet. |
| SMTP | Responsable du périmètre | Configuration du service SMTP pour l'envoi et l'acheminement des courriels. |
| Intégration de la messagerie | Contributeur | Intégration des services de messagerie dans l'architecture globale, en coordination avec l'équipe. |
| Schéma d'architecture et analyse de risques | Contributeur | Participation au schéma d'architecture et contribution à l'analyse de risques du projet. |

## Livrables d'équipe

Le projet inclut notamment :

- DAT et schéma d'architecture ;
- analyse de risques et mesures de sécurité ;
- matrice RACI ;
- inventaire de l'infrastructure virtuelle ;
- conception des services réseau, identité, messagerie, fichiers, supervision, sauvegarde et gestion de parc ;
- dispositifs de détection et tests de sécurité.

## Ajout des identifiants de l'équipe

Les profils GitHub / LinkedIn des membres seront ajoutés dans [TEAM.md](../TEAM.md) uniquement après réception de leurs liens et validation de leur affichage public.
