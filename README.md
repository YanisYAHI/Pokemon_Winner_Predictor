
# 🧠 Pokémon Combat Winner Predictor

A machine learning project that predicts the winner of a Pokémon battle using Pokédex statistics, battle history, and type advantages.

## 🎯 Project Overview

The goal of this project is to build a machine learning model that predicts which Pokémon will win in a one-on-one battle.
The model uses:

 - Pokémon stats

 - Pokémon types

 - historical combat outcomes

 - engineered features related to strengths, weaknesses, and stats differences

The notebook also includes extensive data exploration, cleaning, and type analysis.

## 📦 Dataset

The project relies on three CSV files:

 -  pokemon.csv — contains stats and characteristics of 800 Pokémon

 -  combats.csv — historical battle records (Pokémon 1, Pokémon 2, winner)

 -  tests.csv — unlabeled battles used for final prediction **(lost the file sorry 😶‍🌫️, the syntax should be the same as combats.csv)** 

## 🛠️ Methodology

1. Data Exploration & Cleaning:

   -  Identify Pokémon used/unseen in battles

   -  Analyze type distribution and frequencies

   -  Detect duplicates and missing values:

   -  Build helper structures (ID → type, list of unique types, etc.)

2. Feature Engineering

   -  Extract Pokémon stats and types

   -  Encode categorical attributes

   -  Create engineered combat features (stat differences, type advantage indicators, etc.)

   -  Prepare data for ML (normalization, shaping inputs)

3. Model Training

   -  Train/test split

   -  Supervised training using a classification model (e.g., RandomForest)

   -  Adjust hyperparameters

   -  Evaluate with metrics such as accuracy and confusion matrix

4. Prediction

   -  Apply the trained model to the tests.csv dataset

   -  Generate predicted winners for each match

## 📊 Results

The model is able to:

 -  identify win-prone Pokémon

 -  leverage stat differences and type influences

 -  predict the outcomes of test battles with performance aligned with the dataset’s structure (imbalanced data, stat-heavy outcomes)

## 📁 Repository Structure
```
├── Pokemon_Combat_Winner_Predictor.ipynb   # Main notebook
├── pokemon.csv                             # Pokédex data
├── combats.csv                             # Historical battles
├── tests.csv                               # Battles to predict (still lost 😶‍🌫️)
└── README.md                               # Documentation
```
