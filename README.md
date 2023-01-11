#  Anticipez la consommation électrique et l'émission C02 de bâtiments - Ville de Seattle
#### OpenClassrooms – parcours Data Scientist 
-----
Pour atteindre l'objectif de ville neutre en émissions de carbone en 2050, la ville de Seattle s’intéresse de près à la consommation et aux émissions des bâtiments non destinés à l’habitation. 
Des relevés minutieux ont été effectués en 2015 et en 2016. Cependant, ces relevés sont coûteux à obtenir.

## Mission  
A partir des relevés déjà réalisés en 2015 et 2016 :
* Tenter de prédire les émissions de CO2 et la consommation totale d’énergie de bâtiments non destinés à l’habitation 
* Evaluer l’intérêt du score « ENERGY STAR » pour la prédiction d’émissions 
## Données
- Les données (2015 et 2016) de la ville de Seattle sont à télécharger l’adresse : https://www.kaggle.com/city-of-seattle/sea-building-energy-benchmarking   
- La description des variables est consultable sur la page :https://data.seattle.gov/dataset/2016-Building-Energy-Benchmarking/2bpz-gwpy  
- Le score « Star Energy » est consultable sur le site : https://www.energystar.gov/buildings/benchmark/analyze_benchmarking_results 

Voici le schéma descriptif des données :
<p align="center"><img src="https://github.com/MayChoueib/Projet-Anticipez-la-consommation-electrique-et-l-emission-C02-de-batiments-Ville-de-Seattle/blob/main/schema_donnees.jpg" width="600" height="400" /></p>

## Etapes du projet
Le projet est découpé en deux parties :   
### 1. Notebook_analyse_exploratoire :
Notebook de nettoyage et d’analyse exploratoire des données me permettant de déterminer les variables pertinentes pour la modélisation et les prédictions. Il contient :
-	Nettoyage et visualisation des données
-	Analyse des outliers
-	Analyse de la pertinence des variables
-	Feature engineering

<p align="center"><img src="https://github.com/MayChoueib/Projet-Anticipez-la-consommation-electrique-et-l-emission-C02-de-batiments-Ville-de-Seattle/blob/main/geo_bat.jpg" width="600" height="400" /></p>

### 2. Notebook_Modelisation_Prediction_energie_gaz :

Notebook de modélisations avec des approches linéaires et non-linéaires afin de prédire la consommation énergétique ainsi que les émissions des gaz à effet de serre des bâtiments non destinés à l’habitation (le CO2 est le principal gaz responsable de l'effet de serre). Les étapes sont : 

-	Préparation des données (Séparation des données en données d’entrainement et de test, encodage et standardisation des variables catégorielles)           
-	Modélisation et évaluation :       
 Entrainement de plusieurs modèles :             
•	Linear Regression              
•	Ridge Regression      
•	Lasso Regression       
•	ElasticNet Regression      
•	DecisionTree Regressor      
•	RandomForest Regressor      
•	XGB Regressor        
•	Les métriques utilisées :  RMSE (Root Mean Squared Error), R2 Score (Coefficient of Determination) ainsi que MAE (Mean Absolute Error)       
-	Optimisation des hyperparamètres (Cross validation et GridSearch)      
-	Prédictions sur les données de test       
-	Feature importance et évaluation de l’intérêt du score « ENERGY STAR »          

<p align="center"><img src="https://github.com/MayChoueib/Projet-Anticipez-la-consommation-electrique-et-l-emission-C02-de-batiments-Ville-de-Seattle/blob/main/FE_engyscore.jpg" width="700" height="600" /></p>
