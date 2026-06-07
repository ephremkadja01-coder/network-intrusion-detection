# ML CHALLENGE

Ce dépôt contient un projet de machine learning pour un challenge de données. Il organise l'intégralité du workflow depuis l'analyse exploratoire jusqu'à la préparation des données, l'entraînement de modèles et la génération de soumissions.

## Structure du projet

- `data/`
  - `raw/` : jeux de données bruts, y compris les fichiers d'entraînement, de validation et de test.
- `notebooks/`
  - `01_data_audit.ipynb` : audit initial des données.
  - `02_eda.ipynb` : analyse exploratoire.
  - `03_feature_engineering.ipynb` : construction et transformation des variables.
  - `04_lightgbm.ipynb` : entraînement et évaluation d'un modèle LightGBM.
  - `05_catboost.ipynb` : entraînement et évaluation d'un modèle CatBoost.
  - `06_ensemble.ipynb` : construction d'un modèle d'ensemble.
- `src/`
  - `preprocessing.py` : fonctions de prétraitement des données.
  - `features.py` : génération de features.
  - `train_lightgbm.py` : script d'entraînement LightGBM.
  - `train_catboost.py` : script d'entraînement CatBoost.
  - `predict.py` : script de prédiction et génération de fichier de soumission.
- `models/`
  - `catboost/`, `lightgbm/`, `ensemble/` : modèles sauvegardés ou dossiers de résultats.
- `submission/`
  - fichiers de soumission générés.
- `notes/` et `reports/` : documentation des expériences, hypothèses et visualisations.

## Objectif

L'objectif est de développer une solution robuste pour un challenge de machine learning en :

1. Explorant et auditant les données.
2. Nettoyant et préparant les jeux de données.
3. Construisant des features pertinentes.
4. Entraînant plusieurs modèles (LightGBM, CatBoost, ensemble).
5. Générant des prédictions finales pour la soumission.

## Utilisation

1. Installer les dépendances.

```bash
pip install -r requirements.txt
```

2. Exécuter les notebooks pour comprendre les étapes d'analyse et de feature engineering.

3. Lancer les scripts d'entraînement depuis `src/`.

```bash
python src/train_lightgbm.py
python src/train_catboost.py
```

4. Générer des prédictions.

```bash
python src/predict.py
```

> Remarque : adaptez les entrées et les paramètres selon les scripts et les fichiers de données disponibles.

## Bonnes pratiques

- Vérifier les fichiers de données dans `data/raw/` avant l'entraînement.
- Conserver les versions de modèles dans `models/`.
- Enregistrer les résultats de soumission dans `submission/`.
- Documenter les expériences et les observations dans `notes/`.

## À améliorer

- Compléter `requirements.txt` avec les bibliothèques réellement utilisées.
- Ajouter des instructions détaillées pour l'exécution des scripts et leurs arguments.
- Mettre en place un pipeline plus automatisé si nécessaire.

---

Ce README fournit un guide de base pour naviguer dans le projet et comprendre les composants principaux.
