# 📂 Dossier `data`

Ce dossier contient les fichiers de données fournis par Kaggle pour la compétition *Titanic - Machine Learning from Disaster*.

## 📜 Fichiers disponibles
- `train.csv` : Contient les données d'entraînement avec les labels (`Survived`).
- `test.csv` : Contient les données de test sans les labels.
- `sample_submission.csv` : Exemple de format de soumission pour Kaggle.

## 📥 Utilisation
Avant d'exécuter les notebooks ou scripts Python, assurez-vous que ces fichiers sont bien placés dans ce dossier.

Si les fichiers ne sont pas présents, vous pouvez les télécharger directement depuis la page de la compétition Kaggle :
[Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)

## 🔎 Aperçu des données
Les fichiers CSV contiennent les colonnes suivantes :

### `train.csv`
| PassengerId | Survived | Pclass | Name  | Sex   | Age | SibSp | Parch | Ticket | Fare | Cabin | Embarked |
|------------|---------|--------|------|------|-----|------|------|--------|------|-------|----------|
| 1          | 0       | 3      | John Doe | male  | 22  | 1    | 0    | A/5 21171 | 7.25 | NaN   | S        |

- **Survived** : 0 = Non, 1 = Oui
- **Pclass** : Classe de la cabine (1 = Première, 2 = Deuxième, 3 = Troisième)
- **Sex** : Genre du passager (`male`, `female`)
- **Age** : Âge du passager
- **SibSp** : Nombre de frères/soeurs/conjoints à bord
- **Parch** : Nombre de parents/enfants à bord
- **Fare** : Prix du billet
- **Embarked** : Port d'embarquement (`C = Cherbourg`, `Q = Queenstown`, `S = Southampton`)

### `test.csv`
| PassengerId | Pclass | Name  | Sex   | Age | SibSp | Parch | Ticket | Fare | Cabin | Embarked |
|------------|--------|------|------|-----|------|------|--------|------|-------|----------|
| 892        | 3      | Jane Doe | female | 34  | 0    | 0    | W./C. 6607 | 7.75 | NaN   | Q        |

- Même structure que `train.csv`, sauf que la colonne `Survived` est absente (car elle doit être prédite).

### `sample_submission.csv`
| PassengerId | Survived |
|------------|---------|
| 892        | 0       |
| 893        | 1       |

- Ce fichier montre le format attendu pour la soumission des prédictions sur Kaggle.

## ⚠️ Remarque
Les fichiers `train.csv` et `test.csv` ne sont pas inclus dans le dépôt pour éviter d'enfreindre les règles de Kaggle. Vous devez les ajouter manuellement.

