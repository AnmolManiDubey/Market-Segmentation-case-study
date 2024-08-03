# Market Segmentation Using PCA and KMeans Clustering

## Overview

This repository demonstrates market segmentation through Principal Component Analysis (PCA) and KMeans clustering. The goal is to preprocess the dataset, reduce its dimensionality, identify optimal clusters, and analyze each segment. Additionally, we assess the stability of the clusters and fit a logistic regression model to predict cluster membership.

## Project Steps

### 1. Data Loading and Preprocessing
- **Objective**: Load the dataset and preprocess it for clustering.
- **Actions**:
  - Load the dataset from the source.
  - Convert categorical data to binary using one-hot encoding.
  - Handle any missing values and normalize the data if necessary.

### 2. PCA (Principal Component Analysis)
- **Objective**: Reduce the dimensionality of the dataset and visualize variance.
- **Actions**:
  - Perform PCA to transform the data into principal components.
  - Plot the explained variance to understand the significance of each principal component.

### 3. Optimal Clusters
- **Objective**: Determine the optimal number of clusters for KMeans.
- **Actions**:
  - Use the elbow method to find the optimal number of clusters.
  - Plot the sum of squared distances (inertia) against the number of clusters to identify the elbow point.

### 4. KMeans Clustering
- **Objective**: Apply KMeans clustering to segment the market.
- **Actions**:
  - Fit KMeans clustering to the dataset using the optimal number of clusters.
  - Assign cluster labels to each data point.

### 5. Cluster Analysis
- **Objective**: Analyze and describe each cluster.
- **Actions**:
  - Summarize the characteristics of each cluster.
  - Visualize clusters and interpret the results to understand the market segments.

### 6. Cluster Stability
- **Objective**: Assess the stability of the clusters.
- **Actions**:
  - Use bootstrapping methods to evaluate cluster stability.
  - Calculate the adjusted Rand index to compare cluster results across different runs.

### 7. Regression Model
- **Objective**: Fit a logistic regression model using the clusters.
- **Actions**:
  - Use the cluster labels as target variables.
  - Fit a logistic regression model to predict cluster membership based on features.
  - Evaluate the model's performance and interpret the results.

## Requirements

- Python 3.x
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

## Installation

To set up the environment and install the necessary libraries, you can use the following commands:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
