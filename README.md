README.md
markdown
# Projet : Classification avec Arbres de Décision et Forêts Aléatoires

## 📋 Description
Ce projet implémente des algorithmes de classification (Arbres de Décision et Forêts Aléatoires) sur le dataset Forest Covertypes pour prédire le type de couverture forestière.

## 🎯 Objectifs
- Mettre en œuvre l'algorithme des arbres de décision
- Préparer et prétraiter les données
- Définir des métriques pertinentes
- Comparer avec une baseline simple
- Optimiser les hyperparamètres
- Analyser les résultats et les limites

## 📊 Dataset
**Forest Covertypes** - UCI Machine Learning Repository
- **Échantillons** : 581,012
- **Caractéristiques** : 54 (10 quantitatives + 44 binaires)
- **Classes** : 7 types de couverture forestière
- **Source** : Roosevelt National Forest, Colorado

## 🛠️ Prérequis
- Python 3.8+
- Jupyter Notebook ou Google Colab

## 📦 Installation
```bash
# Cloner le repository
git clone [repository-url]
cd [project-folder]

# Installer les dépendances
pip install -r requirements.txt
Dépendances principales :
text
numpy>=1.21.0
pandas>=1.3.0
scikit-learn>=1.0.0
matplotlib>=3.5.0
seaborn>=0.11.0
scikit-plot>=0.3.7
plotly>=5.6.0
🚀 Exécution
Ouvrir le notebook decision_trees_forest_covertypes.ipynb

Exécuter toutes les cellules dans l'ordre

Les résultats seront affichés directement dans le notebook

Sur Google Colab :
Télécharger le notebook

L'uploader sur Google Colab

Exécuter les cellules (les installations se font automatiquement)

📁 Structure du projet
text
project/
│
├── decision_trees_forest_covertypes.ipynb  # Notebook principal
├── README.md                               # Documentation
├── requirements.txt                        # Dépendances
├── models/                                 # Modèles sauvegardés
│   ├── best_decision_tree.pkl
│   ├── best_random_forest.pkl
│   └── scaler.pkl
└── slides/                                 # Présentation
    └── presentation.pptx
📈 Métriques utilisées
Accuracy : Proportion de prédictions correctes

F1-score : Moyenne harmonique de précision et rappel

Matrice de confusion : Analyse des erreurs par classe

Importance des caractéristiques : Identification des variables importantes

🧪 Modèles implémentés
Baseline : Classifier le plus fréquent

Arbre de décision : Avec optimisation des hyperparamètres

Forêt aléatoire : Avec recherche aléatoire d'hyperparamètres

🔍 Méthodologie
Exploration : Analyse des données et distribution des classes

Prétraitement : Normalisation et encodage

Séparation : Train/Test split (80/20)

Baseline : Établissement d'une performance de référence

Entraînement : Modèles avec paramètres par défaut

Optimisation : Recherche d'hyperparamètres

Évaluation : Métriques et visualisations

Analyse : Interprétation et limites

📊 Résultats
Modèle	Accuracy	F1-score
Baseline	0.486	0.364
Arbre (défaut)	0.856	0.856
Arbre (optimisé)	0.912	0.912
Forêt (défaut)	0.942	0.942
Forêt (optimisée)	0.953	0.953
🔧 Hyperparamètres optimaux
Arbre de décision :
max_depth: 20

min_samples_split: 2

min_samples_leaf: 1

criterion: 'gini'

Forêt aléatoire :
n_estimators: 200

min_samples_split: 2

min_samples_leaf: 1

max_depth: None

bootstrap: True

📝 Interprétation
Caractéristiques importantes : Élévation, pente, distance aux points d'eau

Classes difficiles : Certaines classes sont souvent confondues

Impact du prétraitement : La normalisation améliore significativement les performances

⚠️ Limites identifiées
Déséquilibre des classes affectant les performances sur les classes minoritaires

Complexité computationnelle pour l'optimisation des hyperparamètres

Interprétabilité réduite des forêts aléatoires

Risque de surapprentissage avec des arbres trop profonds

🔮 Améliorations possibles
Techniques de ré-échantillonnage pour le déséquilibre

Essai de modèles de Gradient Boosting

Réduction de dimensionnalité (PCA)

Validation croisée plus poussée

📚 Références
Breiman, L. (2001). Random Forests. Machine Learning, 45(1), 5-32.

Scikit-learn Documentation: https://scikit-learn.org/

UCI Machine Learning Repository: https://archive.ics.uci.edu/ml/datasets/covertype

👥 Auteurs
SOULEIMANI Mohamed Rayan , EL FATTAHI Wissal , OUHMIDOU Amine, BENABDESSADEK Dikra

Ecole Marocaine des Sciences de l'Ingénieurs

📄 Licence
Ce projet est sous licence MIT. Voir le fichier LICENSE pour plus de détails.

