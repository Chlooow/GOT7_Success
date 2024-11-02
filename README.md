# Mini-Projet IAS : GOT7 Song Popularity Prediction

Ce projet vise à prédire le succès des chansons du groupe de K-pop GOT7 en utilisant des techniques d'apprentissage supervisé, telles que la descente de gradient, la régression logistique, le perceptron, PCA/SVM, et l'analyse de la convergence. Ce projet utilise des données fictives, mais repose sur des caractéristiques pertinentes pour prédire la popularité d'une chanson en fonction de diverses métriques. (Mini Projet IAS pour assimiler les connaissances acquises lors du module)

## Table des matières
- Description du Projet
- Données
- Modèles Utilisés
- Méthodologie
- Installation
- Utilisation
- Résultats
- Améliorations Possibles
- Technologies Utilisées

## Description du Projet
Ce projet analyse les chansons de GOT7 en fonction de caractéristiques spécifiques telles que le nombre de vues, les mentions sur les réseaux sociaux, le BPM, la durée, et si la chanson est un "Title Track". L'objectif est de construire un modèle capable de prédire si une chanson sera un succès (succès = 1) ou non (succès = 0).

## Données
Les données comprennent les caractéristiques suivantes pour chaque chanson :

- **Nom de la chanson** : Titre de la chanson.
- **Durée** : Durée de la chanson en secondes.
- **BPM** : Battements par minute (tempo de la chanson).
- **Vues YouTube** : Nombre de vues sur YouTube en millions.
- **Mentions RS** : Nombre de mentions sur les réseaux sociaux en milliers.
- **Title Track** : Indicateur binaire (1 si la chanson est le "Title Track" de l'album).
- **Succès** : Indicateur de succès (1 si la chanson est un succès, 0 sinon).

## Modèles Utilisés
1. **Descente de Gradient** : Pour optimiser les poids d'une régression logistique.
2. **Régression Logistique** : Utilisée pour prédire le succès d'une chanson en fonction des différentes caractéristiques.
3. **Perceptron** : Modèle de classification binaire pour distinguer les succès.
4. **PCA/SVM** : Réduction de la dimensionnalité pour une meilleure classification.
5. **Analyse de la Convergence et de l'Overfitting** : Pour déterminer le nombre optimal d'itérations.

## Méthodologie
- **Préparation des Données** : Les données sont normalisées pour la descente de gradient et divisées en ensembles d'entraînement, de validation, et de test.
- **Descente de Gradient** : Implémentation d'une descente de gradient pour optimiser la fonction de coût.
- **Entraînement et Validation des Modèles** : Entraînement des modèles et évaluation de leur précision.
- **Analyse de Convergence** : Suivi de la fonction de coût pour détecter les signes de sur-apprentissage (overfitting) et identifier le nombre optimal d'itérations.
- **Évaluation des Résultats** : Évaluation du modèle en termes de précision, de rappel, et d'autres métriques si nécessaire.

## Installation
Clonez le dépôt et installez les dépendances nécessaires.
``git clone https://github.com/Chlooow/GOT7_Success
cd GOT7_Success``

Assurez-vous également que les bibliothèques suivantes sont installées :

- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`

## Résultats
Les résultats finaux incluent :

La précision du modèle sur l'ensemble de test.
Les courbes de convergence de la fonction de coût pour visualiser le processus de minimisation.
Analyse des effets du sur-apprentissage sur les résultats.

## Améliorations Possibles
Utilisation d'autres modèles de classification : Comparer avec des modèles comme les forêts aléatoires.
Enrichissement des données : Intégrer davantage de caractéristiques pour chaque chanson.
Optimisation des hyperparamètres : Tester différents taux d'apprentissage et nombres d'itérations.

## Technologies Utilisées
- *Python* : Langage principal pour l'analyse de données et l'apprentissage statistique.
- *NumPy & Pandas* : Manipulation des données.
- *Scikit-learn* : Modèles d'apprentissage automatique.
- *Matplotlib* : Visualisation des résultats.

