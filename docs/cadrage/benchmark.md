# Benchmark des solutions techniques

## Objectif

Cette étude compare les différentes solutions techniques envisageables pour le projet Scribe afin de sélectionner les outils les plus adaptés aux objectifs fonctionnels, techniques et budgétaires.

Les comparaisons portent sur :

* Les plateformes de visioconférence ;
* Les solutions de transcription et diarisation ;
* Les modèles de génération de résumé ;
* Les approches de classification des thèmes et du ton.

---

# 1. Plateformes de visioconférence

## Critères étudiés

* Facilité d'intégration
* Récupération de l'audio
* Documentation
* Coût
* Scalabilité
* Respect du RGPD

| Solution | Audio récupérable | Documentation | Coût     | RGPD | Verdict   |
| -------- | ----------------- | ------------- | -------- | ---- | --------- |
| Jitsi    | Oui               | Bonne         | Gratuit  | Oui  | Très bon  |
| LiveKit  | Oui               | Excellente    | Freemium | Oui  | Excellent |
| Daily    | Oui               | Excellente    | Payant   | Oui  | Très bon  |

---

# 2. Transcription et diarisation

## Critères étudiés

* Qualité de transcription
* Gestion du français
* Diarisation
* Coût
* Rapidité

| Solution           | Français  | Diarisation | Coût    | Verdict   |
| ------------------ | --------- | ----------- | ------- | --------- |
| Whisper + PyAnnote | Excellent | Oui         | Gratuit | Excellent |
| AssemblyAI         | Excellent | Oui         | Payant  | Très bon  |
| Deepgram           | Très bon  | Oui         | Payant  | Très bon  |

---

# 3. LLM pour le résumé

| Solution    | Coût   | Qualité résumé | Facilité API | Verdict     |
| ----------- | ------ | -------------- | ------------ | ----------- |
| GPT-4o-mini | Faible | Excellent      | Excellente   | Recommandé  |
| Mistral     | Faible | Très bon       | Bonne        | Alternative |

---

# 4. Classification des thèmes et du ton

| Solution              | Complexité | Qualité    | Verdict     |
| --------------------- | ---------- | ---------- | ----------- |
| LLM                   | Faible     | Très bonne | Recommandé  |
| Modèle NLP spécialisé | Moyenne    | Bonne      | Alternative |

---

# Recommandation finale

Après analyse, les choix retenus pour le projet Scribe sont :

* Visioconférence : LiveKit
* Transcription : Whisper
* Diarisation : PyAnnote
* Résumé : GPT-4o-mini
* Classification : GPT-4o-mini

Ces solutions offrent le meilleur compromis entre coût, facilité d'intégration, performances et conformité avec les objectifs du projet.
