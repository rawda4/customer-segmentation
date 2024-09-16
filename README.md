# Customer Segmentation Analysis

## Overview
This project aims to perform customer segmentation for an e-commerce platform using unsupervised machine learning techniques, specifically K-Means and Hierarchical Clustering. The goal is to identify customer groups based on their purchasing behavior to enhance marketing strategies and improve customer satisfaction.

## Data Source
The data is sourced from an Excel file named `E-commerce_data.xlsx`, which includes the following sheets:
- **customers**: Contains customer demographic information.
- **genders**: Contains gender-related data.
- **cities**: Contains city information related to customers.
- **transactions**: Contains transaction records.
- **branches**: Contains information about store branches.
- **merchants**: Contains merchant-related data.

## Methodology

### 1. Data Preparation
- The data from various sheets is merged to create a comprehensive dataset.
- Key features are engineered to assess customer behavior, including:
  - Total coupons claimed
  - Recency (days since the last coupon was claimed)
  - Frequency of claims

### 2. Data Standardization
- Standardization of features is performed using `StandardScaler` to ensure that all features contribute equally to the distance calculations in clustering algorithms.

### 3. Clustering Techniques
#### K-Means Clustering
- K-Means clustering is applied to segment customers into distinct groups.
- The optimal number of clusters is determined using the elbow method and silhouette score.

#### Hierarchical Clustering
- Hierarchical clustering is performed to create a dendrogram for visualizing the relationships between clusters.
- The silhouette score is calculated to evaluate the quality of the clusters.

### 4. Visualization
- Scatter plots are created to visualize both K-Means and Hierarchical clustering results, illustrating how customers are grouped based on their purchasing behavior.

## Results
- The analysis produces segments of customers characterized by their purchasing behavior metrics.
- Silhouette scores are provided for both clustering methods to assess the clustering quality.
