/!\ Etant donné la confidentialité des données, celles-ci ont été supprimées du repo public afin de ne présenter que la modélisation /!\

## Contexte

Réalisé dans le cadre d'un hackathon d'une semaine courant mars 2025, ce notebook propose l'étude d'un jeu de données `features.csv` et la modélisation de sa relation avec les variables cibles `output1_1w` et `output1_1m`.  
Face à la nature des données, l'approche retenue a été un entraînement semi-supervisé d'un modèle `RandomForestRegressor` et d'un ensemble de modèles optimisé par Autogluon (framework AutoML).  
Les deux variables cibles ont été traitées séparément, avec les résultats suivants :

- **output1_1w**
  - Mean Squared Error : **2.77**
  - R² Score : **0.49**

- **output1_1m**
  - Mean Squared Error : **4.07**
  - R² Score : **0.71**

Pour atteindre ces résultats, plusieurs approches ont été explorées (apprentissage supervisé, dépendance temporelle, régression linéaire, techniques d’imputation et de traitement des données).  
Cependant, pour des raisons de clarté, seule l’approche la plus performante est présentée dans le notebook.

Plusieurs visualisations ont également été réalisées afin de confirmer ou infirmer certaines intuitions, mais ne figurent pas dans la version finale du notebook.

## Bibliothèques Utilisées

### Bibliothèques Standards

- **pandas** : manipulation et analyse des données
- **numpy** : opérations numériques
- **matplotlib** : visualisation des données
- **seaborn** : visualisations statistiques avancées
- **sklearn** : machine learning
- **statsmodels** : modèles statistiques et tests

### Bibliothèques Non Standards

- **fancyimpute** : imputation des valeurs manquantes
- **autogluon** : automation du machine learning

---

## Installation

Pour installer les bibliothèques nécessaires, utilisez le fichier `requirements.txt` fourni :

```bash
pip install -r requirements.txt
```

Ou bien exécutez la cellule suivante dans votre notebook :

```python
!pip install pandas numpy matplotlib seaborn scikit-learn statsmodels fancyimpute autogluon
```

---

## Fichiers

- `features.csv` : Jeu de données utilisé
- `notebook.ipynb` : Notebook principal
- `requirements.txt` : Dépendances Python

---

## Remarques

- Les résultats sont reproductibles sur CPU avec les hyperparamètres indiqués dans le notebook.
- Pour toute question ou amélioration, n’hésitez pas à me contacter.
