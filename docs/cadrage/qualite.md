# Plan Qualité

## Objectif

Garantir la qualité du projet Scribe tout au long du développement en définissant des règles de développement, des indicateurs de qualité et une stratégie de tests.

---

## Revue de code

Chaque fonctionnalité est développée dans une branche dédiée (`feature/*`).

Avant intégration dans la branche `develop` :

* Vérification du code ;
* Vérification du respect des conventions de nommage ;
* Vérification des tests associés ;
* Vérification de la documentation.

---

## Standards de développement

* Python 3.12
* Respect de la norme PEP8
* Utilisation de type hints
* Documentation des fonctions principales
* Commits conventionnels (`feat`, `fix`, `docs`, `test`, `refactor`)

---

## Stratégie de tests

### Tests unitaires

* Validation des fonctions métier
* Validation des appels API
* Validation du traitement des données

### Tests d'intégration

* Vérification des échanges entre FastAPI et les services IA
* Vérification des accès à la base de données

---

## Objectifs de qualité

| Indicateur                 | Objectif     |
| -------------------------- | ------------ |
| Couverture de tests        | ≥ 70 %       |
| Taux de réussite des tests | 100 %        |
| Temps moyen de réponse API | < 3 secondes |
| Taux d'erreurs critiques   | 0            |

---

## Intégration Continue

Le projet utilisera GitHub Actions afin d'exécuter automatiquement :

* Linting du code ;
* Exécution des tests ;
* Vérification de la qualité avant fusion dans `develop`.
