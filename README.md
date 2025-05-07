# London Houses Clustering Analysis

This project analyzes a dataset of houses in London to identify meaningful clusters based on physical characteristics of the properties. The dataset includes 1,000 records with features such as the number of bedrooms, bathrooms, square meters, building age, garden, garage, floors, and property type. The goal is to group similar houses without using subjective or derived attributes such as price or interior style.

## Dimensionality Reduction

To better visualize the data and understand its structure, three dimensionality reduction methods were applied:
- **PCA** (Principal Component Analysis)
- **t-SNE** (t-distributed Stochastic Neighbor Embedding)
- **ICA** (Independent Component Analysis)

Visual inspection of the reduced data suggested an optimal number of clusters between **4 and 12**, with **12** being the more consistent value across methods.

## Clustering Methods

The following clustering algorithms were used:
- **K-Means**
- **DBSCAN**
- **Agglomerative Clustering**
- **Gaussian Mixture Models**

### Key Findings:
- **DBSCAN** and **Agglomerative Clustering** identified **12 clusters** and performed best both visually and according to clustering quality metrics.
- **K-Means** and **Gaussian Mixture** tended to identify only **4 clusters**, showing lower internal cohesion and cluster separation.

## Evaluation Metrics

Metrics used to assess cluster quality:
- **Silhouette Score**
- **Calinski-Harabasz Index**
- **Davies-Bouldin Index**

Results confirmed that DBSCAN and Agglomerative Clustering achieved higher Silhouette Scores and lower Davies-Bouldin values, indicating better-defined clusters.

---
