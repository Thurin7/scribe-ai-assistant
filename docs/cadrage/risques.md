# Plan de Risques

## Matrice des risques

| ID  | Risque                                                               | Probabilité | Criticité   | Impact potentiel                                                                                          | Mesures préventives                                                         |
| --- | -------------------------------------------------------------------- | ----------- | ----------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| R1  | Non-conformité RGPD                                                  | Moyenne     | Très élevée | Sanctions de la CNIL, atteinte à l'image de l'entreprise, suspension du service                           | Consentement explicite, durée de conservation limitée, droit à l'effacement |
| R2  | Fuite de données ou accès non autorisé                               | Faible      | Très élevée | Divulgation d'informations confidentielles, perte de confiance des utilisateurs, responsabilité juridique | Authentification sécurisée, chiffrement, gestion des accès                  |
| R3  | Dépassement du budget API IA                                         | Moyenne     | Élevée      | Augmentation des coûts d'exploitation, modèle économique non viable                                       | Suivi des coûts, quotas, optimisation des appels IA                         |
| R4  | Indisponibilité d'un fournisseur externe (OpenAI, Whisper API, etc.) | Moyenne     | Élevée      | Interruption partielle ou totale du service                                                               | Prévoir des solutions alternatives et mécanismes de reprise                 |
| R5  | Erreur dans la transcription ou la diarisation                       | Moyenne     | Élevée      | Comptes-rendus inexacts, mauvaise attribution des décisions et actions                                    | Validation utilisateur, amélioration continue des modèles                   |
| R6  | Contestation de l'enregistrement d'une réunion                       | Faible      | Élevée      | Litiges juridiques, suppression forcée des données                                                        | Écran de consentement obligatoire avant captation                           |
| R7  | Temps de traitement trop long                                        | Moyenne     | Moyenne     | Dégradation de l'expérience utilisateur, baisse de l'adoption du produit                                  | Optimisation des traitements, découpage des fichiers longs                  |
| R8  | Perte ou corruption des données stockées                             | Faible      | Élevée      | Perte de l'historique des réunions et des comptes-rendus                                                  | Sauvegardes régulières et restauration automatisée                          |
| R9  | Faible adoption par les utilisateurs                                 | Moyenne     | Moyenne     | Retour sur investissement limité et abandon du produit                                                    | Interface simple, tests utilisateurs et amélioration UX                     |
| R10 | Dépendance excessive à un seul fournisseur IA                        | Moyenne     | Moyenne     | Difficulté à changer de solution ou hausse soudaine des coûts                                             | Architecture modulaire permettant de remplacer les APIs                     |

## Risques prioritaires

Les risques prioritaires pour le projet Scribe sont :

1. R1 – Non-conformité RGPD ;
2. R2 – Fuite de données sensibles ;
3. R3 – Dépassement du budget API ;
4. R4 – Dépendance aux fournisseurs externes ;
5. R5 – Qualité insuffisante des transcriptions.

Ces risques feront l'objet d'un suivi particulier lors des phases de développement et de mise en production.
