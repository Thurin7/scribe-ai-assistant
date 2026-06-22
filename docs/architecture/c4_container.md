# Diagramme C4 - Niveau Container

## Objectif

Le diagramme Container décrit l'architecture interne de Scribe.

## Containers

### Frontend Streamlit

Responsabilités :

* Interface utilisateur
* Upload audio
* Consultation des réunions
* Affichage des résultats

### API FastAPI

Responsabilités :

* Gestion des requêtes
* Orchestration des traitements IA
* Communication avec la base de données

### Module Whisper

Responsabilités :

* Transcription audio

### Module PyAnnote

Responsabilités :

* Attribution des locuteurs

### Module OpenAI

Responsabilités :

* Résumé automatique
* Extraction d'actions
* Classification

### PostgreSQL

Responsabilités :

* Persistance des données

## Flux

Utilisateur
↓
Streamlit
↓
FastAPI
├── Whisper
├── PyAnnote
├── OpenAI
└── PostgreSQL
