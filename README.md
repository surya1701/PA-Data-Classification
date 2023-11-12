# PA-Data-Classification
## Problem Statement
Can we develop a predictive model for forecasting the outcomes of International Football/Soccer games based on historical data?

The objective is to to predict the outcome of football matches before-hand by using suitable data about the Countries/Teams that are playing each other.

## Data Sources
- Matches dataset from 2006-2018 (Team Country Names, Match Date, Competition Name, Goals scored by both teams)
- Squad dataset of individual competitions (Country, Coach Name, Player Name, Position, Caps)
- FIFA rating  (Team Country Names, Match Date, Competition Name, Goals scored by both teams)
- Year-wise Population of Countries (Country, Population from 1960-2022)
- Year-wise GDP of Countries (Country, GDP from 1960-2021)
- Year-wise average years of schooling in Countries (Country, Continent, ISO Code, avg years of schooling from 1990-2021)

## Preprocessing
- Replaced Missing Values
- Outlier Detection based on COF
- Normalization
- Encoding (nominal to numeric)

## Modelling
|Model   | Score (%)|
|-------- |-----------|
|KNN      |52.21|
|SVM      |53.53|
|DT       |50.46|
|RF       |55.92|
|**GB**   |**56.69**|
|NN       |52.70|
## RapidMiner Screenshots
<div style="width:100">
  <img src="Results/Screenshot 2023-11-11 230947.png" width="30%" />
  <img src="Results/Screenshot 2023-11-11 231003.png" width="30%" />
  <img src="Results/Screenshot 2023-11-11 231023.png" width="30%" />
</p>
  
## Folder Contents
    .
    ├── model.rmp               # RapidMiner model
    ├── Final_Data.csv          # Combined dataset
    ├── Final_Data_pre.csv      # Combined and pre-processed dataset
    ├── Data Collection.ipynb   # Code for data cleaning and combining
    ├── Football                # Football data
    │   ├── ...                 # matches, squads, players, fifa ratings
    ├── Countries               # Country-specific data
    │   ├── ...                 # GDP, Population, Average years of schooling
    ├── Results                 # Prediction files for individual models and Grid Search
    │   ├── <model>.csv         # Training file
    │   ├── <model>.txt         # Accuracy and Confusion Matrix
    ├── KNN Scratch.ipynb       # Code for KNN implemented form scratch
    └── ...
