# Project Big Data - Supervised Learning

## Introduction

Ce projet a été réalisé sur **Databricks** et vise à utiliser **Apache Spark MLlib** pour résoudre un problème de classification binaire : **prédire si le revenu annuel d'un individu est supérieur à 50 000 $** en s'appuyant sur des données démographiques. Le dataset, constitué de **32 561 enregistrements**, est issu du *UCI Machine Learning Repository* et est fourni avec le Databricks Runtime.

## Objectifs

Les principaux objectifs de ce projet sont :
- Explorer les outils et fonctionnalités de **Spark MLlib** pour le traitement de données, la création de pipelines de machine learning et l'optimisation de modèles.
- Comparer les performances de deux modèles de classification (**SVM** et **Random Forest**) pour la prédiction de revenus.
- Analyser l'importance des variables et déterminer si un modèle basé sur un sous-ensemble de variables pertinentes peut offrir des performances similaires.

## Contenu du Projet

Ce notebook est structuré selon les étapes suivantes :

1. **Chargement des données** : Importation et analyse initiale du jeu de données.
2. **Nettoyage des données** : Préparation des données pour l'apprentissage, en traitant les valeurs manquantes et les incohérences.
3. **Définition des modèles** : Configuration des modèles de classification à tester.
4. **Construction du pipeline** : Création d'un pipeline complet intégrant prétraitement, modélisation et évaluation.
5. **Évaluation des modèles** : Comparaison des modèles à l'aide de métriques telles que la courbe ROC, le F1-Score et le rappel (Recall).
6. **Réglage des hyperparamètres** : Optimisation des paramètres pour maximiser la performance.
7. **Prédictions finales** : Utilisation des modèles optimisés pour effectuer des prédictions sur des données de test.
8. **Sélection de variables** : Identification des variables les plus pertinentes et évaluation d'un modèle simplifié.

## Méthodes de Classification et Évaluation

Les deux modèles de classification testés sont :
- **Support Vector Machine (SVM)**
- **Random Forest**

### Métriques d'évaluation

Les performances des modèles sont comparées selon les critères suivants :
- **Courbe ROC** : évaluation de la capacité de discrimination du modèle.
- **F1-Score** : mesure de l'équilibre entre précision et rappel.
- **Recall (rappel)** : proportion de vrais positifs correctement identifiés.

L'objectif est d'identifier le meilleur modèle en termes de performance et d'explorer si un modèle simplifié, basé sur un sous-ensemble de variables pertinentes, peut être aussi performant.

## Prérequis et Installation

### Prérequis

Pour exécuter ce projet, assurez-vous d'avoir les éléments suivants :
- **Apache Spark** avec la bibliothèque **MLlib**
- **Databricks** comme environnement compatible Spark
- **Python 3.x**

### Installation

1. **Clonez le dépôt** :
   ```bash
   git clone <URL_du_dépôt>
   cd Project_Big_Data_Supervised_Learning
