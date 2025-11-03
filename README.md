# 🧠 Lab – Hidden Markov Models (HMM)

## 📘 Description
Ce notebook fait partie du cours **Machine Learning 2** (Degree in Data Science and Engineering, Fall 2024).  
Il explore en profondeur les **Hidden Markov Models (HMM)**, un modèle probabiliste séquentiel utilisé pour modéliser des données temporelles ou symboliques.  
Les exemples et exercices ont été adaptés par *Jose Manuel de Frutos Porras* et *David Martínez Rubio* à partir du travail de *Ignacio Peis* (Dept. of Signal Processing and Communications).

---

## 🧩 Contenu principal

### 1. Introduction  
Présentation des **Markov Models** et introduction des **variables latentes** pour former un modèle caché (HMM).  

### 2. Hidden Markov Models  
- Définition formelle du modèle : états cachés, observations, probabilités de transition et d’émission.  
- Schéma de la structure probabiliste.  
- Notations :  
  - \( A \): matrice de transition  
  - \( B \): distribution d’émission  
  - \( \pi \): distribution initiale  

#### 2.1. Inference  
Explication des principaux algorithmes :
- **Forward** : calcul de la probabilité d’une séquence observée.  
- **Forward-Backward** : estimation des marges lissées.  
- **Viterbi** : recherche de la séquence d’états la plus probable.

#### 2.2. Learning – Baum-Welch Algorithm  
Apprentissage des paramètres \( A, B, \pi \) via l’algorithme **EM** adapté aux HMM :
- Étape **E** : calcul des espérances (γ, ξ).  
- Étape **M** : mise à jour des paramètres du modèle.  
- Cas **gaussien** et **discret** abordés.

#### 2.3. Fully Observed HMMs  
Version simplifiée où les états sont connus — calcul direct du maximum de vraisemblance.

#### 2.4. HMMs avec `hmmlearn`  
Présentation de la bibliothèque Python [`hmmlearn`](https://hmmlearn.readthedocs.io) : création, entraînement et génération de séquences HMM.

---

## 🧪 3. Expérimentations – Human Activity Recognition (HAR)
Application pratique des HMM à la **reconnaissance d’activités humaines** à partir de données capteurs (base *DaLiAc*).  
- Prétraitement des données (fenêtrage, extraction de moyennes/écarts types).  
- Apprentissage d’un HMM gaussien avec `hmmlearn`.  
- Visualisation de la **matrice de transition** \( A \) et interprétation des activités.  

---

## ⚙️ Librairies utilisées
- `numpy`  
- `pandas`  
- `matplotlib`  
- `scikit-learn`  
- `hmmlearn`

---

## 🎯 Objectif
- Comprendre la structure et le fonctionnement des HMM.  
- Implémenter les algorithmes d’inférence et d’apprentissage.  
- Appliquer un HMM à des données réelles (reconnaissance d’activité).

---
