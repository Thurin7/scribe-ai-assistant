# Analyse RGPD & Éthique IA

## Contexte

L'application Scribe collecte et traite des données personnelles issues des réunions professionnelles. Ces données comprennent les voix des participants, les échanges verbaux, les transcriptions générées ainsi que les comptes-rendus produits par les modèles d'intelligence artificielle.

Certaines de ces données peuvent être considérées comme sensibles car elles permettent d'identifier directement ou indirectement une personne.

---

## Données traitées

### Données collectées

* Nom de l'utilisateur
* Adresse e-mail
* Audio des réunions
* Transcriptions
* Comptes-rendus
* Actions attribuées
* Métadonnées de réunion

### Données sensibles

Les enregistrements vocaux peuvent être assimilés à des données biométriques lorsqu'ils permettent d'identifier un individu.

---

## Consentement des participants

Avant chaque réunion, un écran de consentement informe les participants que :

* la réunion est enregistrée ;
* les échanges sont transcrits ;
* les données peuvent être analysées par des services d'IA ;
* les données seront conservées pendant une durée limitée.

Le consentement doit être accepté avant le démarrage de l'enregistrement.

---

## Durée de conservation

Les données seront conservées pendant une durée maximale de 12 mois.

À l'expiration de cette période, les enregistrements audio et les transcriptions seront supprimés automatiquement.

---

## Droit à l'effacement

L'utilisateur pourra demander la suppression :

* d'une réunion ;
* d'une transcription ;
* d'un compte-rendu.

La suppression entraînera l'effacement définitif des données associées.

---

## Sous-traitants et services tiers

Le projet utilise potentiellement :

* OpenAI (génération de résumé)
* Mistral AI
* APIs de transcription

Avant la mise en production, une vérification des conditions de traitement des données et des accords de sous-traitance (DPA) devra être réalisée.

---

## Analyse des risques

| Risque                                | Impact | Mesure                          |
| ------------------------------------- | ------ | ------------------------------- |
| Fuite d'un enregistrement             | Élevé  | Chiffrement et contrôle d'accès |
| Accès non autorisé aux comptes-rendus | Élevé  | Authentification                |
| Conservation excessive des données    | Moyen  | Suppression automatique         |
| Erreur d'attribution d'un locuteur    | Moyen  | Validation utilisateur          |

---

## Mesures retenues

### Socle

* Information des participants
* Durée de conservation définie
* Suppression manuelle des réunions

### Cible

* Écran de consentement dédié
* Analyse des risques
* Journalisation des accès

### Avancé

* Anonymisation automatique
* Droit à l'effacement automatisé
* Gestion complète des demandes RGPD
