# Diagramme C4 - Niveau Contexte

## Objectif

Le diagramme C4 de niveau Contexte présente les interactions entre les utilisateurs du système Scribe et les systèmes externes utilisés pour le traitement des réunions.

## Acteurs

### Utilisateur

L'utilisateur crée, consulte et analyse ses réunions via l'application Scribe.

## Système principal

### Scribe

Application web intelligente permettant :

* la captation audio ;
* la transcription ;
* l'identification des locuteurs ;
* l'analyse des thèmes ;
* la génération de comptes-rendus ;
* la gestion de l'historique des réunions.

## Systèmes externes

### Whisper

Service de transcription audio vers texte.

### PyAnnote

Service de diarisation permettant d'identifier les différents intervenants.

### OpenAI

Service utilisé pour générer les résumés, détecter les thèmes et extraire les actions.

### PostgreSQL

Base de données utilisée pour stocker les utilisateurs, réunions, transcriptions et comptes-rendus.

## Vue simplifiée

Utilisateur
↓
Scribe
├── Whisper
├── PyAnnote
├── OpenAI
└── PostgreSQL
