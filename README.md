# portfolio-data-project
Analyse et visualisation des prix des maisons avec Python

## Description
Ce projet explore le dataset **AmesHousing** afin de comprendre les facteurs qui influencent le prix des maisons.  
L'analyse se concentre sur la relation entre la **surface du premier étage** et le **prix de vente**, en comparant deux quartiers représentatifs : North Ames (NAmes) et College Creek (CollgCr).

Le projet montre comment :  
- Nettoyer et préparer des données immobilières réelles  
- Analyser la relation linéaire entre variables  
- Visualiser des tendances avec des graphiques 
- Identifier et traiter l’impact des valeurs extrêmes sur la modélisation  

---

## Objectifs
- Explorer les distributions de prix et de surfaces dans deux quartiers distincts  
- Quantifier la relation entre surface du premier étage et prix de vente avec le coefficient de corrélation de Pearson  
- Visualiser les résultats avec des nuages de points et lignes de régression  
- Préparer les données pour une modélisation future en utilisant la transformation logarithmique sur le prix  

---

## Technologies Utilisées
- **Python**  
- **Pandas / NumPy** → manipulation et calcul sur les données  
- **Matplotlib** → visualisations statiques  
- **Scipy** → calcul de corrélations statistiques  
- **Jupyter Notebook** → workflow interactif et reproductible  

---

## Contenu du Repository
- `AmesHousing.ipynb` : Notebook principal avec nettoyage, analyse, visualisations et corrélation  
- `README.md` : description détaillée du projet
- Dataset `AmesHousing.csv

---

## Analyse et Résultats
-**Visualisation des distributions des prix de vente**
les distributions des prix de vente entre North Ames et College Creek sont significativement différentes. Les deux quartiers ne présentent pas la même distribution de valeurs.
- **Corrélation Prix vs Surface** :  
  - North Ames (NAmes) : r = 0.52 (corrélation modérée)  
  - College Creek (CollgCr) : r = 0.63 (corrélation plus forte)  
- La corrélation est **positive et significative** dans les deux quartiers : plus la surface augmente, plus le prix augmente.  
- Les **valeurs extrêmes** peuvent fausser les résultats, d’où l’utilisation du **log(prix)** pour une modélisation plus fiable.  

- **Visualisations** :  
  - Nuages de points avec lignes de régression pour chaque quartier  
  - Comparaison côte à côte des tendances des deux quartiers  
  

---

## Instructions pour Utiliser le Projet
1. Télécharger le fichier `AmesHousing_Analysis.ipynb`  
2. Ouvrir avec Jupyter Notebook 
3. Exécuter les cellules pour explorer les données, visualisations et résultats  


---

## Insights pour Modélisation Future
- La surface du premier étage est un bon prédicteur du prix, mais l’effet des **outliers** doit être neutralisé  
- L’utilisation de log(SalePrice) permet de respecter les hypothèses de linéarité et de normalité pour les modèles de régression  
- Cette approche peut être étendue à d’autres variables : qualité globale, année de construction, nombre de chambres, etc.  

---

## Dataset
Le dataset `AmesHousing.csv`.  
Il contient les informations sur les maisons à Ames, notamment :  
- Prix de vente (`SalePrice`)  
- Surface du premier étage (`1st Flr SF`)  
- Quartier (`Neighborhood`)  
- Et d’autres caractéristiques des maisons (année de construction, nombre de chambres, qualité globale, etc.)  

Le fichier CSV est inclus dans ce repository dans le dossier `data/`

---

**Auteur :** Nassima Redouane  
**Objectif :** Portfolio de Data Science pour stage coop



