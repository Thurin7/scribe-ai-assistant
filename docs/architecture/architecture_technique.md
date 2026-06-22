# Architecture Technique

## Vue d'ensemble

Le projet Scribe repose sur une architecture modulaire séparant :

- Frontend
- Backend
- Services IA
- Base de données

---

## Frontend

### Technologie

- Streamlit

### Responsabilités

- Authentification
- Upload audio
- Consultation des réunions
- Dashboard

---

## Backend

### Technologie

- FastAPI

### Responsabilités

- API REST
- Gestion des utilisateurs
- Gestion des réunions
- Orchestration IA

---

## Services IA

### Whisper

- Transcription audio

### PyAnnote

- Diarisation

### GPT-4o-mini

- Résumé
- Extraction d'actions
- Classification

---

## Base de données

### PostgreSQL

Tables principales :

- User
- Meeting
- Speaker
- TranscriptSegment
- Theme
- ActionItem

---

## Déploiement

### Développement

- Docker Compose

### Production

- Render ou Railway

---

## CI/CD

### GitHub Actions

Pipeline :

- Lint
- Tests
- Build
- Déploiement

---

## Monitoring

Prévu pour le niveau avancé :

- Logs centralisés
- Alertes
- Suivi des performances