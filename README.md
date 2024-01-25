# CryptoClustering
Module 19 Challenge

## Description
This project involved using Python and unsupervised learning to predict if cryptocurrencies were affected by different time period price changes (24-hour, 7-day, etc..). The primary goal was to implement the K-means clustering algorithm and explore the impact of using original scaled data versus PCA (Principal Component Analysis) data for clustering.

## Components

### 1. Data Preparation
  - Loaded the crypto_market_data.csv into a DataFrame.
  - Obtained summary statistics and ploted the data to understand its structure.
  - Normalized the data using the StandardScaler module from scikit-learn.
  - Created a DataFrame with scaled data, setting "coin_id" as the index.

### 2. Found Best Value for k Using Original Scaled DataFrame
  - Implemented the elbow method to find the optimal value for k.
  - Plotted the elbow curve to visually identify the best value for k.
  - Estimated the best value for k

### 3. Clustered Cryptocurrencies with K-means Using Original Scaled Data
  - Initialized the K-means model with the best value for k.
  - Fitted the model using the original scaled DataFrame.
  - Predicted clusters and created a scatter plot with hvPlot, showcasing the results.

### 4. Optimized Clusters with Principal Component Analysis (PCA)
  - Performed PCA on the original scaled DataFrame to reduce features to three principal components.
  - Retrieved explained variance to understand the contribution of each principal component.
  - Created a new DataFrame with PCA data, setting "coin_id" as the index.

### 5. Found Best Value for k Using PCA Data
  - Applied the elbow method to find the optimal value for k using PCA data.
  - Plotted the elbow curve to visually identify the best value for k.
  - Estimated the best value for k when using PCA data.

### 6. Clustered Cryptocurrencies with K-means Using PCA Data**
  - Initialized the K-means model with the best value for k using PCA data.
  - Fitted the model using the PCA data.
  - Predicted clusters and created a scatter plot with hvPlot, highlighting the impact of using fewer features for clustering.

## Files
- **Final_Code-folder**
  - **Resources-folder**
    - crypto_market_data.csv
  
  - Crypto_Clustering.ipynb

## Table of Contents
- [CryptoClustering](#cryptoclustering)
  - [Description](#description)
  - [Components](#components)
    - [1. Data Preparation](#1-data-preparation)
    - [2. Finding Best Value for k Using Original Scaled DataFrame](#2-finding-best-value-for-k-using-original-scaled-dataframe)
    - [3. Clustered Cryptocurrencies with K-means Using Original Scaled Data](#3-clustered-cryptocurrencies-with-k-means-using-original-scaled-data)
    - [4. Optimizing Clusters with Principal Component Analysis (PCA)](#4-optimizing-clusters-with-principal-component-analysis-pca)
    - [5. Finding Best Value for k Using PCA Data](#5-finding-best-value-for-k-using-pca-data)
    - [6. Clustering Cryptocurrencies with K-means Using PCA Data](#6-clustering-cryptocurrencies-with-k-means-using-pca-data)
  - [Files](#files)
