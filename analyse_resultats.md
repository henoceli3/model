# Analyse des Résultats de la Prédiction du Taux de Congestion à Abidjan

## 1. Analyse Exploratoire des Données

### Distribution du Taux de Congestion

- Les données montrent une distribution inégale des taux de congestion
- La majorité des observations se situent dans les niveaux moyens à élevés
- Peu de cas de congestion très faible

### Relation Affluence-Congestion

- Forte corrélation positive entre l'affluence et le taux de congestion
- La présence de chantiers influence cette relation
- Plus l'affluence est élevée, plus le taux de congestion tend à augmenter

### Impact des Conditions Météorologiques

- Les conditions orageuses sont associées à des taux de congestion plus élevés
- La météo nuageuse montre des taux de congestion variables
- Les conditions ensoleillées présentent généralement des taux de congestion plus modérés

### Effet des Chantiers

- La présence de chantiers augmente généralement le taux de congestion
- Impact plus marqué dans certaines communes que d'autres

## 2. Évaluation des Modèles

### Performances Comparées

1. **Gradient Boosting** (Meilleur modèle)

   - R² = 0.533 (53.3% de variance expliquée)
   - RMSE = 0.620
   - MAE = 0.461

2. **Ridge Regression**

   - R² = 0.524
   - RMSE = 0.626
   - MAE = 0.515

3. **Linear Regression**

   - R² = 0.503
   - RMSE = 0.639
   - MAE = 0.527

4. **Random Forest**

   - R² = 0.458
   - RMSE = 0.667
   - MAE = 0.434

5. **Lasso**

   - R² = 0.329
   - RMSE = 0.743
   - MAE = 0.592

6. **Decision Tree**

   - R² = 0.068
   - RMSE = 0.876
   - MAE = 0.433

7. **SVR**
   - R² = -0.391
   - RMSE = 1.069
   - MAE = 0.687

### Importance des Features

Les features les plus influentes sont :

1. **Affluence** (49.86%) : De loin le facteur le plus important
2. **Météo Orageuse** (21.32%) : Deuxième facteur le plus influent
3. **Présence d'Événement** (5.98%) : Impact modéré
4. **Météo Nuageuse** (5.62%) : Impact similaire aux événements
5. **Heure** (5.34%) : Influence notable sur la congestion

## 3. Conclusions

1. **Choix du Modèle**

   - Le Gradient Boosting offre les meilleures performances globales
   - Bonne balance entre précision et généralisation
   - Supérieur aux approches linéaires traditionnelles

2. **Facteurs Clés**

   - L'affluence est le prédicteur dominant
   - Les conditions météorologiques ont un impact significatif
   - L'heure de la journée joue un rôle important

3. **Limites du Modèle**

   - Performance modérée (R² = 0.533)
   - Marge d'amélioration possible
   - Certains facteurs peuvent être manquants

4. **Recommandations**
   - Collecter plus de données pour améliorer la précision
   - Considérer l'ajout de nouvelles variables
   - Explorer des approches d'ensemble plus sophistiquées
