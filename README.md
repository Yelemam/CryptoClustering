# CryptoClustering
# Cryptocurrency Clustering with K-Means and PCA

## Project Overview

This project applies unsupervised learning techniques, specifically K-Means clustering, to analyze and group cryptocurrencies based on their price change 
percentages over different timeframes. Principal Component Analysis (PCA) is used to optimize the clustering by reducing the dimensionality of the dataset. 
The project aims to explore whether cryptocurrencies are affected by price changes over 24-hour and 7-day periods.

## Table of Contents

1. Project Overview
2. Technologies Used
3. Installation and Setup
4. Usage
5. Elbow Method and Clustering Resuts
6. Visualizations
7. Acknowledgments

## Technologies Used

- Python
- Jupyter Notebook
- Scikit-learn
- hvPlot
- Matplotlib
- Pandas
- Principal Component Analysis (PCA)
- K-Means Clustering

## Installation and Setup

1. Clone the repository to your local machine:
    ```bash
    git clone <repository-url>
    
2. Navigate to the project folder:
    ```bash
    cd CryptoClustering
    
3. Open the Jupyter Notebook:
    ```bash
    jupyter notebook
    

## Usage

1. Open the `Crypto_Clustering.ipynb` notebook.
2. Follow the steps to load the cryptocurrency data and normalize it using `StandardScaler`.
3. Apply the K-Means clustering algorithm on both the original data and the PCA-transformed data.
4. Visualize the results of the elbow method and the cryptocurrency clusters.
5. Compare the clustering results before and after applying PCA to evaluate the impact of dimensionality reduction.

## Elbow Method and Clustering Results

Used the Elbow Method to determine the optimal number of clusters for grouping cryptocurrencies. The best value for `k` was found to be 4, both in 
the original scaled data and the PCA-transformed data.

Using K-Means clustering, the cryptocurrencies were grouped based on their 24-hour and 7-day price change percentages. The use of PCA helped optimize 
the clustering process by reducing the number of features, while retaining 89.50% of the original data's variance.

## Visualizations

1. **Elbow Curves**: These are used to identify the optimal number of clusters (`k`).
    - [Original Data Elbow Curve](images/elbow_plot.png)
    - [PCA Data Elbow Curve](images/elbow_plot_pca.png)

2. **Cluster Visualizations**: These show how the cryptocurrencies are grouped based on K-Means clustering.
    - [Original Data Cluster Plot](images/crypto_clusters.html)
    - [PCA Data Cluster Plot](images/pca_crypto_clusters.html)

3. **Composite Visualizations**: Comparisons of the elbow curves and clustering results with and without PCA.
    - [Composite Elbow Plot](images/composite_elbow_plot.png)
    - [Composite Cluster Plot](images/composite_cluster_plot.html)

## Acknowledgments

This project was developed as part of the Module 19 Challenge for cryptocurrency clustering. Special thanks to the open-source libraries and tools 
that made this project possible.

Additionally, I would like to acknowledge the use of AI assistance through OpenAI’s ChatGPT to help problem-solving, and rewording sentences in the project.

