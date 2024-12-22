# CryptoClustering

This project uses **unsupervised machine learning techniques** to analyze and cluster cryptocurrencies based on their performance metrics. By leveraging **K-Means clustering** and **Principal Component Analysis (PCA)**, we identify distinct clusters of cryptocurrencies that exhibit similar price change patterns.

---

## Objectives

1. Perform data preprocessing and normalization on cryptocurrency data.
2. Identify the optimal number of clusters (k) using the **Elbow Method**.
3. Cluster cryptocurrencies using the **K-Means algorithm**.
4. Optimize clustering by reducing dimensionality with **Principal Component Analysis (PCA)**.
5. Visualize and compare clusters from original data and PCA-reduced data.

---

## Technologies Used

- **Python**
- **Pandas**
- **Scikit-learn**: 
- **hvPlot**
- **Jupyter Notebook**

---

## Files

- **`Crypto_Clustering.ipynb`**: The main notebook containing all the steps of the project.
- **`crypto_market_data.csv`**: Dataset used for the analysis, containing cryptocurrency price change percentages over different time periods.
- **README.md**: Documentation for the project.

---

## Methodology

### 1. Data Preprocessing
- Load the cryptocurrency dataset.
- Normalize the data using `StandardScaler`.

### 2. Elbow Method
- Use the **Elbow Method** to determine the optimal number of clusters (`k`) by plotting inertia values for different cluster sizes (1–11).
- Optimal `k` was found to be **4**.

### 3. K-Means Clustering
- Perform clustering using K-Means on the normalized data.
- Assign cluster labels to each cryptocurrency.

### 4. Dimensionality Reduction with PCA
- Reduce the dataset to **three principal components** using PCA.

### 5. Optimized Clustering
- Reapply the K-Means algorithm to the PCA-reduced data.
- Compare clusters from the PCA data to those from the original data.

---

## Visualizations

### Elbow Curves
- **Original Data**: 
- **PCA Data**: 

### Cluster Comparison
- Scatter plots were created for:
  - Original scaled data (`price_change_percentage_24h` vs. `price_change_percentage_7d`).
  - PCA-reduced data (`PCA1` vs. `PCA2`).
- Clusters are well-separated in both plots, with clearer separation in the PCA plot.

---

## How to Run the Notebook

1. Clone the repository:
   ```bash
   git clone https://github.com/nanis911/CryptoClustering.git
