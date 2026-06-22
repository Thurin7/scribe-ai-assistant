# Plan de Risques

## Objectif

Identifier les principaux risques du projet Scribe afin de mettre en place des mesures préventives et correctives dès la phase de pré-production.

## Matrice des risques

| ID | Risque                                 | Probabilité | Impact     | Criticité | Mesures                                                      |
| -- | -------------------------------------- | ----------- | ---------- | --------- | ------------------------------------------------------------ |
| R1 | Dépassement du budget API              | Moyenne     | Élevé      | Élevée    | Utiliser des modèles économiques, surveiller la consommation |
| R2 | Latence importante de transcription    | Moyenne     | Élevé      | Élevée    | Tests de performance, limitation de la taille des fichiers   |
| R3 | Mauvaise qualité de diarisation        | Moyenne     | Moyenne    | Moyenne   | Évaluation sur plusieurs jeux de données                     |
| R4 | Échec de l'intégration visio           | Faible      | Élevé      | Moyenne   | Prévoir une maquette simulée pour le Sprint 0                |
| R5 | Défaillance d'un service externe (API) | Moyenne     | Élevé      | Élevée    | Prévoir des alternatives et gestion d'erreurs                |
| R6 | Non-conformité RGPD                    | Faible      | Très élevé | Élevée    | Consentement, durée de conservation, suppression             |
| R7 | Perte ou corruption des données        | Faible      | Élevé      | Moyenne   | Sauvegardes régulières                                       |
| R8 | Retard dans le développement           | Moyenne     | Moyenne    | Moyenne   | Priorisation du backlog et respect des sprints               |

---

## Représentation simplifiée

| Impact / Probabilité | Faible | Moyenne    | Élevée |
| -------------------- | ------ | ---------- | ------ |
| Faible               | R7     |            |        |
| Moyenne              |        | R3, R8     |        |
| Élevée               | R4     | R1, R2, R5 | R6     |

---

## Risques prioritaires

Les risques considérés comme prioritaires pour le projet sont :

* Dépassement du budget API ;
* Latence de transcription ;
* Défaillance des services tiers ;
* Conformité RGPD.

Ces risques feront l'objet d'un suivi régulier durant les sprints de développement.
