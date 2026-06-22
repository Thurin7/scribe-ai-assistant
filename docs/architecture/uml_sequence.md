# UML de Séquence - Traitement d'une réunion

## Objectif

Décrire le traitement complet d'une réunion depuis la captation audio jusqu'à la génération du compte-rendu final.

---

# Scénario 1 : Mode Dictaphone

Acteurs :

- Utilisateur
- Streamlit
- FastAPI
- Whisper
- PyAnnote
- OpenAI
- PostgreSQL

## Séquence

Utilisateur
→ Streamlit : Démarre l'enregistrement

Streamlit
→ FastAPI : Envoie le fichier audio

FastAPI
→ Whisper : Transcription audio

Whisper
→ FastAPI : Texte transcrit

FastAPI
→ PyAnnote : Identification des locuteurs

PyAnnote
→ FastAPI : Segments diarises

FastAPI
→ OpenAI : Résumé + Actions + Thèmes

OpenAI
→ FastAPI : Compte-rendu structuré

FastAPI
→ PostgreSQL : Sauvegarde

PostgreSQL
→ FastAPI : Confirmation

FastAPI
→ Streamlit : Affichage du résultat

---

# Scénario 2 : Mode Visioconférence

Acteurs :

- Utilisateur
- Plateforme Visio
- FastAPI
- Whisper
- PyAnnote
- OpenAI
- PostgreSQL

## Séquence

Utilisateur
→ Plateforme Visio : Participe à la réunion

Plateforme Visio
→ FastAPI : Flux audio

FastAPI
→ Whisper : Transcription

Whisper
→ FastAPI : Texte

FastAPI
→ PyAnnote : Attribution des locuteurs

PyAnnote
→ FastAPI : Résultat

FastAPI
→ OpenAI : Résumé + Actions + Thèmes

OpenAI
→ FastAPI : Compte-rendu

FastAPI
→ PostgreSQL : Sauvegarde

FastAPI
→ Utilisateur : Consultation du résultat