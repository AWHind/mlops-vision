# MLOps Vision

Projet **MLOps de bout en bout en Computer Vision**, couvrant l’ensemble du cycle de vie d’un projet de Machine Learning, de la préparation des données jusqu’au déploiement et au suivi du modèle.

## 🎯 Objectifs du projet

L’objectif est de développer et d’industrialiser une solution de Computer Vision en appliquant les bonnes pratiques MLOps :

* 📊 Préparer, nettoyer et valider les données
* 🧠 Développer et entraîner un modèle de Computer Vision
* 📈 Évaluer les performances du modèle
* 🔬 Suivre et comparer les expérimentations
* 🏷️ Versionner les modèles et les expériences
* ⚙️ Automatiser le pipeline de Machine Learning
* 🚀 Déployer le modèle à travers une API
* 📡 Surveiller les performances du modèle
* 🔄 Garantir la reproductibilité et la maintenabilité du projet

## 🏗️ Architecture du projet

```text
Données
   │
   ▼
Préparation & Validation
   │
   ▼
Exploration & Prétraitement
   │
   ▼
Entraînement du modèle
   │
   ▼
Évaluation & Suivi des expériences
   │
   ▼
Versionnement du modèle
   │
   ▼
Déploiement via API
   │
   ▼
Monitoring
```

## 📁 Structure du projet

```text
mlops-vision/
│
├── data/
│   ├── raw/                 # Données brutes
│   └── processed/           # Données prétraitées
│
├── models/                  # Modèles entraînés
│
├── notebooks/               # Exploration et expérimentations
│
├── src/
│   ├── data/                # Prétraitement des données
│   ├── models/              # Entraînement des modèles
│   └── ...                  # Composants du pipeline ML
│
├── tests/                   # Tests unitaires et d'intégration
│
├── configs/                 # Fichiers de configuration
│
├── scripts/                 # Scripts d'automatisation
│
├── .github/
│   └── workflows/           # Workflows CI/CD
│
├── .gitignore
├── .pre-commit-config.yaml
├── README.md
└── requirements.txt
```

## 🛠️ Technologies utilisées

* **Python**
* **PyTorch / TorchVision**
* **OpenCV**
* **Scikit-learn**
* **Pandas / NumPy**
* **Matplotlib**
* **FastAPI**
* **MLflow**
* **Git / GitHub**
* **Pre-commit**
* **Pytest**

## 🔀 Stratégie Git

Le projet adopte une stratégie Git adaptée aux projets de Machine Learning :

* `main` → branche stable du projet
* `feature/*` → développement de nouvelles fonctionnalités
* `experiment/*` → expérimentations et tests de modèles

Des **tags Git annotés** sont utilisés pour identifier les versions importantes du projet et les différentes étapes expérimentales.

## 🔐 Qualité du code et sécurité

Des hooks **pre-commit** permettent d'automatiser plusieurs contrôles avant chaque commit :

* **Black** → formatage automatique du code Python
* **check-added-large-files** → détection des fichiers volumineux
* **nbstripout** → suppression des sorties des notebooks
* **Détection des secrets** → détection des clés API, tokens et mots de passe potentiels
* **Validation des messages de commit** → respect d'une convention de nommage

## 🚀 Installation

Cloner le dépôt puis créer un environnement virtuel :

```bash
git clone <repository-url>
cd mlops-vision

python -m venv .venv
```

### Activation avec Git Bash

```bash
source .venv/Scripts/activate
```

### Activation avec PowerShell

```powershell
.venv\Scripts\Activate.ps1
```

Installer les dépendances :

```bash
pip install -r requirements.txt
```

## 🧪 Tests et vérifications

Exécuter les tests du projet :

```bash
pytest
```

Exécuter l'ensemble des contrôles pre-commit :

```bash
pre-commit run --all-files
```

## 📌 État actuel du projet

Le projet comprend actuellement :

* ✅ Initialisation du dépôt Git
* ✅ Structure d'un projet MLOps
* ✅ Jeu de données et notebook d'exploration
* ✅ Branches dédiées aux expérimentations
* ✅ Tags Git annotés
* ✅ Rebase interactif et squash
* ✅ Résolution des conflits lors d'un rebase
* ✅ Contrôles de qualité avec pre-commit
* ✅ Protection contre les fichiers volumineux
* ✅ Nettoyage automatique des notebooks
* ✅ Détection des secrets
* ✅ Validation des messages de commit

## 🔜 Prochaines étapes

* Développer le modèle de Computer Vision
* Mettre en place l'entraînement et l'évaluation automatisés
* Intégrer **MLflow** pour le suivi des expérimentations
* Développer l'API d'inférence avec **FastAPI**
* Mettre en place une **CI/CD avec GitHub Actions**
* Ajouter le monitoring du modèle


