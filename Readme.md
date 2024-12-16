# Data Mining Project

## Overview
This project analyzes traffic collision data in New York City using advanced data mining techniques to uncover meaningful insights. The main objectives are:

1. **Predicting Missing Motivations**: Developing a Random Forest classification model to estimate unspecified collision causes.
2. **Identifying Collision Patterns**: Using clustering techniques to find patterns and categorize collisions based on shared characteristics.

## Dataset
The dataset used for this project includes detailed records of traffic collisions in New York City between 2016 and 2023. Key attributes include:
- **Location Details**: Borough, ZIP code, latitude, longitude, and street names.
- **Incident Information**: Date, time, number of injuries and fatalities (pedestrians, cyclists, motorists).
- **Collision Causes**: Various motivations contributing to the accidents.

The dataset was processed and manipulated using Python libraries such as Pandas and external tools like the OpenStreetMap API to fill missing location data.

## Methodology

### 1. Data Preparation
- **Column Merging**: Consolidated street names and removed redundant columns.
- **Error Correction**: Fixed missing or incorrect spatial and numeric values.
- **Outlier Removal**: Filtered invalid data points based on geographic boundaries.

### 2. Data Visualization
Visualized key patterns and distributions using:
- Monthly trends in collision counts.
- Heatmaps for spatial distribution of accidents.
- Bar charts categorizing injuries and fatalities.

### 3. Dimensionality Reduction
- **Word2Vec**: Reduced the number of unique motivations by grouping similar ones based on cosine similarity.
- **PCA**: Used Principal Component Analysis to reduce dimensionality for clustering.

### 4. Supervised Learning
- Implemented a **Random Forest classifier** to predict unspecified collision motivations.
- Conducted hyperparameter tuning and tested class balancing strategies.

### 5. Clustering
- Applied the **K-Medoids algorithm** to identify collision patterns.
- Optimized the number of clusters using Elbow and Silhouette methods.

## Key Results
- Successfully predicted missing motivations with a Random Forest model, achieving an accuracy of ~36%.
- Identified 15 distinct clusters of collisions, categorized by severity (high, medium, low) and characteristics such as time, location, and vehicle type.

## Societal Impact
The findings reveal:
- Brooklyn and Queens as high-risk boroughs.
- The significant role of driver inattention as a cause of collisions.
- Insights to guide infrastructure improvements, like bike lanes and awareness campaigns.

## Authors
- Stefano Baroni
- Matteo Mormile