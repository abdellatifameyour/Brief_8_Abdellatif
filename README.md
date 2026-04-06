# 📊 Projet Data Analyst – Analyse Statistique & Applications Métier

## 🧭 Contexte du projet

Dans le cadre de ce projet, j’interviens en tant que **Data Analyst junior** sur différentes problématiques métiers, avec pour objectif de :

* Comprendre et maîtriser les concepts statistiques fondamentaux
* Appliquer ces concepts à des datasets réels
* Produire des analyses fiables, interprétables et utiles à la prise de décision

Ce projet est structuré autour de **deux cas d’usage principaux** :

1. Analyse de données de **santé publique**
2. Analyse de données **automobiles (dataset MPG)**


## 🎯 Objectifs pédagogiques

À l’issue de ce projet, je suis capable de :

* Définir et expliquer les concepts statistiques clés
* Distinguer les **variables discrètes** et **continues**
* Réaliser des **analyses descriptives** complètes
* Produire des **visualisations pertinentes** (histogramme, boxplot, etc.)
* Identifier et interpréter les **valeurs aberrantes (outliers)**
* Mesurer les relations entre variables (**corrélation**)
* Réaliser des **tests d’hypothèses** et interpréter les résultats
* Faire le lien entre théorie statistique et problématiques métiers

---

## 🧠 Phase 1 – Compréhension & Documentation

### 📌 Statistiques descriptives

* **Moyenne (Mean)** : valeur centrale moyenne d’une distribution
* **Médiane (Median)** : valeur centrale qui sépare les données en deux
* **Variance** : mesure de dispersion autour de la moyenne
* **Écart-type** : racine de la variance (dispersion interprétable)
* **Histogramme** : visualisation de la distribution des données
* **Boxplot** : détection des outliers et résumé statistique


### 📌 Population vs Échantillon

* **Population** : ensemble complet des données
* **Échantillon** : sous-ensemble représentatif
* Importance : réduire le coût et le temps d’analyse
* Risques : biais d’échantillonnage


### 📌 Probabilités et distributions

* **Bernoulli** : événement binaire (succès/échec)
* **Binomiale** : répétition d’expériences Bernoulli
* **Poisson** : événements rares dans le temps
* **Normale** : distribution en cloche (très fréquente)
* **Student (t)** : petits échantillons
* **Chi-deux** : test d’indépendance


### 📌 Théorème Central Limite (TCL)

* La moyenne d’échantillons suit une **loi normale**, même si la population ne l’est pas
* Permet de faire des **inférences statistiques**
* Fondamental pour les tests d’hypothèses


### 📌 Échantillonnage et estimation

* Estimation d’une population via un échantillon
* Types de biais :

  * Biais de sélection
  * Biais de mesure
* Importance de la représentativité

---

### 📌 Tests d’hypothèses

* **H0 (hypothèse nulle)** : pas d’effet / pas de relation
* **H1 (hypothèse alternative)** : effet présent
* **p-value** : probabilité d’obtenir le résultat observé si H0 est vraie
* Décision :

  * p-value < α → rejet de H0
  * p-value ≥ α → non rejet

---

## ⚙️ Phase 2 – Analyse du Dataset Santé

### 🔍 Typologie des variables

* Variables **discrètes** : Country, Year
* Variables **continues** : Spending_USD, Life_Expectancy

---

### 📊 Analyse des variables

#### Country

* Variable qualitative
* Permet des comparaisons entre pays

#### Spending_USD

* Analyse de la distribution
* Moyenne = dépense moyenne en santé par habitant
* ⚠️ Interprétation précise :

  > La moyenne représente le montant moyen dépensé par habitant pour la santé sur la période étudiée

#### Life_Expectancy

* Analyse de la distribution
* Évolution dans le temps
* Comparaison entre pays

---

### 📈 Analyses demandées

* Histogramme + Boxplot pour chaque variable
* Évolution temporelle (line plot)
* Comparaison Allemagne vs Royaume-Uni
* Analyse spécifique par pays

---

### 🔗 Relation entre variables

* Relation entre **Spending_USD** et **Life_Expectancy**
* Cas spécifique : États-Unis (2000–2020)

#### Corrélation de Pearson

* Mesure de la force de la relation linéaire
* Interprétation :

  * proche de 1 → forte corrélation positive
  * proche de 0 → aucune relation

---

### ⚠️ Valeur aberrante

* Détection via boxplot
* Une valeur extrême peut fausser :

  * moyenne
  * corrélation

---

### 🧪 Test d’hypothèse (Bonus)

Hypothèse :

* H0 : augmentation = 0.3/an

* H1 : augmentation ≠ 0.3

* Calcul avec `.diff()`

* Niveau de confiance : 98% (α = 0.02)

---

## 🚗 Phase 3 – Analyse Dataset MPG

### 🔍 Typologie des variables

* **Discrètes** :

  * cylinders
  * origin
  * model_year

* **Continues** :

  * mpg
  * horsepower
  * weight
  * acceleration

---

### 📊 Analyse des variables

#### mpg (consommation)

* Moyenne = consommation moyenne des voitures

* ⚠️ Interprétation :

  > Représente le nombre moyen de miles parcourus par gallon de carburant

* Graphiques :

  * Histogramme
  * Boxplot

---

### 🔎 Analyses clés

* mpg vs horsepower → relation inverse
* Ajout de model_year → amélioration dans le temps
* Évolution du poids (USA 1970–1982)
* Relation :

  * cylinders vs year
  * cylinders vs origin

---

### 🌍 Comparaisons

* Accélération moyenne par pays
* Focus sur l’année 1980
---

## 🛠️ Outils utilisés

* Python (Pandas, NumPy)
* Matplotlib / Seaborn
* Jupyter Notebook

---

## 📌 Conclusion

Ce projet permet de passer de la **théorie statistique** à une **application concrète métier**, en développant des compétences essentielles en :

* Analyse de données
* Interprétation statistique
* Visualisation
* Prise de décision basée sur les données
