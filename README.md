# Titanic - Machine Learning from Disaster

## Description
Ce projet est une participation à la compétition Kaggle "Titanic: Machine Learning from Disaster". L'objectif est d'entraîner un modèle de Machine Learning capable de prédire la survie des passagers du Titanic en fonction des caractéristiques fournies.

## 📂 Structure du projet
```
📂 **Titanic-Kaggle-Competition**
├── 📂 **models/**
│   ├── 📂 **v1/**
│   │   ├── 📄 model.pkl
│   │   ├── 📄 train.py
│   │   ├── 📄 predict.py
│   │   ├── 📄 evaluate.py
│   │   ├── 📄 config.yaml
│   ├── 📂 **v2/**
│   │   ├── 📄 model.pkl
│   │   ├── 📄 train.py
│   │   ├── 📄 predict.py
│   │   ├── 📄 evaluate.py
│   │   ├── 📄 config.yaml
│   ├── 📄 __init__.py
├── 📂 **data/**
│   ├── 📂 **raw/**
│   ├── 📂 **processed/**
│   ├── 📄 train.csv
│   ├── 📄 test.csv
│   ├── 📄 __init__.py
├── 📂 **utils/**
│   ├── 📄 preprocessing.py
│   ├── 📄 feature_engineering.py
│   ├── 📄 metrics.py
│   ├── 📄 logger.py
│   ├── 📄 __init__.py
├── 📂 **tests/**
│   ├── 📄 test_predict.py
│   ├── 📄 test_evaluate.py
│   ├── 📄 test_preprocessing.py
│   ├── 📄 __init__.py
├── 📂 **notebooks/**
│   ├── 📄 eda.ipynb
│   ├── 📄 model_training.ipynb
│   ├── 📄 evaluation.ipynb
├── 📂 **scripts/**
│   ├── 📄 train.sh
│   ├── 📄 evaluate.sh
│   ├── 📄 preprocess.sh
├── 📂 **logs/**
│   ├── 📄 training.log
│   ├── 📄 predictions.log
├── 📄 main.py
├── 📄 config.yaml
├── 📄 requirements.txt
├── 📄 README.md
├── 📄 Dockerfile
├── 📄 Makefile
├── 📄 .gitignore
├── 📂 **.github/**
│   ├── 📂 **workflows/**
│   │   ├── 📄 ci.yml


## 📊 Données
Les fichiers de données fournis par Kaggle sont stockés dans le répertoire `data/` :
- `train.csv` : Jeu d'entraînement
- `test.csv` : Jeu de test
- `sample_submission.csv` : Exemple de soumission

## 🚀 Installation
1. Cloner le dépôt :
   ```sh
   git clone https://github.com/votre-utilisateur/Titanic-Kaggle-Competition.git
   cd Titanic-Kaggle-Competition
   ```
2. Installer les dépendances :
   ```sh
   pip install -r requirements.txt
   ```

## 📘 Utilisation
### Prétraitement des données
```sh
python scripts/preprocess.py
```
### Entraînement du modèle
```sh
python scripts/train_model.py
```
### Prédictions
```sh
python scripts/predict.py
```

## 📝 Fichiers essentiels
### 📂 data/README.md
```markdown
# 📂 Dossier `data`
Ce dossier contient les fichiers de données fournis par Kaggle pour la compétition Titanic.

## 📜 Fichiers disponibles
- `train.csv` : Données d'entraînement
- `test.csv` : Données de test
- `sample_submission.csv` : Exemple de format de soumission

Les fichiers doivent être placés ici avant d'exécuter les notebooks et scripts du projet.
```

### 📂 .gitignore
```gitignore
__pycache__/
data/
models/
*.pkl
*.log
*.csv
*.ipynb_checkpoints/
```

### 📂 requirements.txt
```txt
numpy
pandas
matplotlib
seaborn
scikit-learn
jupyter
```

### 📂 LICENSE
```txt
MIT License

Copyright (c) 2025 Rayan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

[...]
```

### 📂 config.yaml
```yaml
settings:
  random_seed: 42
  test_size: 0.2
  model:
    type: "RandomForestClassifier"
    n_estimators: 100
    max_depth: None
  paths:
    train_data: "data/train.csv"
    test_data: "data/test.csv"
    model_output: "models/best_model.pkl"
```

## 📜 Licence
Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 📬 Contact
Si vous avez des questions, n'hésitez pas à me contacter sur Kaggle ou GitHub !


