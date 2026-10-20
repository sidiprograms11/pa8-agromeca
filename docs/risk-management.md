# Synthèse de l'analyse de risques

## Méthode

L'équipe a recensé les processus métier, les biens supports, les événements redoutés, les scénarios de menace et les mesures de sécurité. Chaque risque est évalué selon son impact et sa vraisemblance, puis réévalué après prise en compte des contrôles existants.

L'analyse couvre **31 scénarios** et articule les besoins de :

- confidentialité ;
- intégrité ;
- disponibilité ;
- détection et réponse.

## Risques prioritaires et réponses de sécurité

| Risque | Impacts visés | Réponse d'architecture |
| --- | --- | --- |
| Vol de comptes, phishing et accès distant frauduleux | Confidentialité, intégrité | Identité centralisée, politiques de mots de passe, certificats, MFA selon le service, journalisation et sensibilisation. |
| Ransomware et perte de données | Disponibilité, intégrité | Segmentation, protection des postes, sauvegardes isolées, versioning et alertes sur le chiffrement massif. |
| Vol ou fuite de plans CAO | Confidentialité, propriété intellectuelle | Isolation du périmètre ingénierie, contrôle d'accès, chiffrement, traçabilité et sensibilisation. |
| Modification de plans ou de données de production | Intégrité, sûreté métier | Droits fondés sur les rôles, segmentation, versioning, supervision et alertes de modification. |
| Compromission d'un service web exposé | Confidentialité, disponibilité | Reverse proxy, filtrage applicatif, exposition minimale, supervision et correctifs. |
| Mouvement latéral interne | Confidentialité, intégrité, disponibilité | Segmentation inter-zones, filtrage au moindre privilège et visibilité centralisée. |
| Défaillance de sauvegarde ou de restauration | Disponibilité | Sauvegardes quotidiennes, stockage séparé, alertes et tests de restauration. |
| Manque de visibilité sur les incidents | Détection et réponse | Collecte de journaux, corrélation SIEM, IDS/HIDS et alertes sur les sources manquantes. |

## Détection et supervision

La stratégie de détection rassemble les événements d'authentification, les actions d'administration, le filtrage réseau, les journaux web, les services de messagerie, les accès aux fichiers et les échecs de sauvegarde. L'objectif est d'associer prévention et détection, plutôt que de se limiter au blocage.

Les scénarios sont rapprochés de tactiques pertinentes de MITRE ATT&CK, notamment l'accès initial, l'accès aux identifiants, l'exécution, la découverte, le mouvement latéral, la collecte, l'impact et le commandement et contrôle.

## Apprentissage clé

Un pare-feu seul ne suffit pas. La réduction du risque dépend de contrôles complémentaires : segmentation, identité, chiffrement, supervision, sauvegarde, procédures et responsabilités clairement attribuées.

## Limites de publication

Les scores détaillés, preuves de configuration, actifs précis et mesures de détection exactes ne sont pas publiés. Cette synthèse permet d'évaluer la démarche sans augmenter la surface d'attaque du projet.
