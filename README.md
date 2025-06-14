# Preprocessing BMGs Dataset - Data Mining Project

Ce projet a été réalisé dans le cadre du module **Data Mining**.  
Il concerne le prétraitement d’un jeu de données sur des **alliages métalliques amorphes (BMGs - Bulk Metallic Glasses)**.


## Contenu du projet

Ce notebook Google Colab contient les étapes suivantes :

### 1. Chargement et exploration des données
- Chargement du fichier CSV
- Affichage des premières lignes
- Vérification des colonnes et types de données

### 2. Nettoyage
- Suppression des lignes/colonnes inutiles
- Gestion des valeurs manquantes
- Uniformisation des formats de données

### 3. Traitement de la colonne `composition`
- Extraction des éléments chimiques (`Ag`, `Ca`, `Mg`, `Cu`, etc.)
- Gestion des formules complexes du type `{[(Fe60 Co40)75 B20 Si5]96 Nb4}99 Cr1`
- Séparation en colonnes individuelles par élément

### 4. Détection des outliers
- Analyse avec Z-score uniquement sur les colonnes physiques :
  - `Tg`, `Tx`, `Tl`, `Dmax`
- Visualisation des valeurs extrêmes (boxplots, histogrammes)

### 5. Normalisation
- Normalisation par **Z-score** des colonnes numériques
- Création de nouvelles colonnes `*_z` pour chaque variable


## Objectif final

Préparer un dataset propre et prêt pour l’étape suivante du projet :  
> **Le clustering avec l’algorithme K-Means.**

## 🛠️ Technologies utilisées

- Python 3.x  
- Google Colab  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- Scikit-learn  
