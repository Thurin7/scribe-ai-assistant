# ERD - Modèle de données

## Objectif

Le modèle de données permet de stocker les utilisateurs, les réunions, les transcriptions, les locuteurs identifiés ainsi que les actions et thèmes extraits automatiquement.

---

# Entités

## User

| Attribut | Type |
|-----------|---------|
| id | UUID |
| email | VARCHAR |
| password_hash | VARCHAR |
| created_at | TIMESTAMP |

---

## Meeting

| Attribut | Type |
|-----------|---------|
| id | UUID |
| user_id | UUID |
| title | VARCHAR |
| meeting_type | VARCHAR |
| audio_path | TEXT |
| created_at | TIMESTAMP |

Relation :
- Un utilisateur possède plusieurs réunions.

---

## Speaker

| Attribut | Type |
|-----------|---------|
| id | UUID |
| meeting_id | UUID |
| label | VARCHAR |

Relation :
- Une réunion possède plusieurs locuteurs.

---

## TranscriptSegment

| Attribut | Type |
|-----------|---------|
| id | UUID |
| meeting_id | UUID |
| speaker_id | UUID |
| start_time | FLOAT |
| end_time | FLOAT |
| content | TEXT |

Relation :
- Une réunion possède plusieurs segments.
- Un segment appartient à un locuteur.

---

## Theme

| Attribut | Type |
|-----------|---------|
| id | UUID |
| meeting_id | UUID |
| name | VARCHAR |

Relation :
- Une réunion peut posséder plusieurs thèmes.

---

## ActionItem

| Attribut | Type |
|-----------|---------|
| id | UUID |
| meeting_id | UUID |
| description | TEXT |
| owner | VARCHAR |
| due_date | DATE |
| status | VARCHAR |

Relation :
- Une réunion possède plusieurs actions.

---

# Relations

User
│
└── Meeting
      │
      ├── Speaker
      ├── TranscriptSegment
      ├── Theme
      └── ActionItem