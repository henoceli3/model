# Projet de Prédiction du Taux de Congestion à Abidjan

## Description du Projet

Ce projet vise à prédire le taux de congestion dans différentes communes d'Abidjan en utilisant des techniques d'apprentissage automatique. L'objectif est d'aider à la gestion du trafic urbain et à la planification des déplacements.

## Structure du Projet

```
code/model/
├── predition_taux_congestion.ipynb   # Notebook principal
├── analyse_resultats.md              # Analyse détaillée des résultats
├── best_model.joblib                 # Modèle sauvegardé
└── columns.joblib                    # Colonnes pour le prétraitement
```

## Données Utilisées

- **Points de ralentissement** : Localisation géographique des points de congestion
- **Variables temporelles** : Heures, dates, jours de la semaine
- **Conditions** : Météo, événements, présence de chantiers
- **Mesures** : Affluence et taux de congestion

## Modèles Testés

1. Gradient Boosting (meilleur modèle)
2. Ridge Regression
3. Linear Regression
4. Random Forest
5. Lasso
6. Decision Tree
7. SVR

## Résultats Principaux

- **Meilleur Modèle** : Gradient Boosting
  - R² : 0.533
  - RMSE : 0.620
  - MAE : 0.461

## Features Importantes

1. Affluence (49.86%)
2. Conditions météorologiques orageuses (21.32%)
3. Événements (5.98%)
4. Météo nuageuse (5.62%)
5. Heure de la journée (5.34%)

## Installation et Utilisation

1. Cloner le repository
2. Installer les dépendances :

```bash
pip install -r requirements.txt
```

3. Ouvrir le notebook `predition_taux_congestion.ipynb`
4. Exécuter les cellules dans l'ordre

## Dépendances Principales

- Python 3.8+
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn
- jupyter

## Auteurs et Contribution

- KODJO TAMEGNON ELISEE HENOC @henoceli3
- N'ZI CEDRIC

## Licence

[Type de licence]
