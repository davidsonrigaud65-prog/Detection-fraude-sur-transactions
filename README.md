##Détection de Fraude Bancaire (ML Supervisé)

Ce projet présente un pipeline complet de Machine Learning capable de traiter des données transactionnelles brutes et bruitées pour identifier des comportements frauduleux.


 Objectif
Développer un modèle robuste capable de maximiser la détection des fraudes (Recall) tout en gérant un dataset déséquilibré et complexe (formats hétérogènes, doublons, erreurs de saisie).


 Points Forts du Projet
1. Data Engineering & Nettoyage
Normalisation multi-sources : Conversion automatique des devises (USD vers HTG) et nettoyage des formats de dates hétérogènes.


Traitement du bruit : Suppression des doublons, correction des types de données et standardisation des variables catégorielles (ex: villes).


2. Pipeline Anti-Fuite (Anti-Leakage)
Utilisation de Scikit-Learn Pipeline pour garantir que le prétraitement (Scaling, Imputation) est appris uniquement sur le jeu d'entraînement.


Split Stratifié : Conservation du ratio de fraude entre les sets d'entraînement et de test.


3. Modélisation & Optimisation
Modèle : Régression Logistique avec régularisation L1 (Lasso).

Stratégie de classe : Utilisation de class_weight='balanced' pour compenser le déséquilibre des données.

Seuils de décision : Analyse des courbes Precision-Recall pour permettre un ajustement métier (priorité au Rappel pour ne manquer aucune fraude).

 Résultats Clés
Recall (Fraude) : 1.00 (en ajustant le seuil à 0.15).

Pipeline : 100% reproductible et prêt pour de nouveaux types de modèles (Random Forest, XGBoost).


 Stack Technique
Python • Pandas • Scikit-Learn • Matplotlib • Seaborn


Pourquoi ce projet est-il pertinent ?
Il démontre ma capacité à transformer des données réelles "sales" en un système de prédiction fiable, en respectant scrupuleusement les bonnes pratiques du Machine Learning pour éviter le sur-apprentissage.
