# Clustering Analysis on Wholesale Customers Dataset

## 📅 Overview
This project conducts a comprehensive comparative analysis of clustering algorithms on the **Wholesale Customers Dataset** from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/machine-learning-databases/00292/Wholesale%20customers%20data.csv). We explore how different clustering methods and preprocessing techniques affect clustering performance.

### 🌐 Clustering Algorithms Implemented:
- **K-Means Clustering**
- **Agglomerative (Hierarchical) Clustering**
- **Mean-Shift Clustering**

### ⚖️ Preprocessing Techniques Applied:
- Raw Data (No preprocessing)
- Standard Scaling
- Power Transformation
- PCA (Principal Component Analysis)

---

## 📊 Dataset Description
The dataset includes annual spending (in monetary units) of clients on various product categories:
- **Fresh**
- **Milk**
- **Grocery**
- **Frozen**
- **Detergents_Paper**
- **Delicassen**

Total number of data points: **440**  
Number of features used: **6**

---

## ⚙️ Methodology & Implementation

### 💡 Preprocessing Steps:
- **Standard Scaling**: Rescales features to have a mean of 0 and a standard deviation of 1.
- **Power Transformation**: Reduces skewness and makes data distribution more Gaussian-like.
- **PCA**: Reduces dimensionality to improve visualization and potentially enhance clustering quality.

### 📊 Evaluation Metrics:
To assess the performance of each clustering method, we used:

1. **Silhouette Score** – Measures how similar an object is to its own cluster vs. other clusters.
2. **Calinski-Harabasz Index** – Assesses separation between clusters (higher is better).
3. **Davies-Bouldin Index** – Evaluates average similarity between clusters (lower is better).

### 📈 Outputs Generated:

- `clustering_results.csv`: Contains all performance scores (Silhouette, Calinski-Harabasz, Davies-Bouldin) for each algorithm and preprocessing combination.
- **Visualizations**:
  - `KMeans_clusters.png`
  - `Hierarchical_clusters.png`
  - `MeanShift_clusters.png`
  - `dendrogram.png` for Hierarchical clustering

---

## 🔄 Sample Visual Results

### 📅 K-Means Clustering
![K-Means Clusters](https://github.com/user-attachments/assets/545fac4a-9686-4f20-b954-ec9185f344c0)

### 📅 Hierarchical Clustering Dendrogram
![Dendrogram](https://github.com/user-attachments/assets/bc4fa015-6dc9-43d0-9b2f-a1655a8b17d7)

---

## 🚀 Conclusion

After evaluating all clustering methods and preprocessing combinations:

- **Best Clustering Algorithm**: `KMeans`
- **Best Number of Clusters**: `3`
- **Best Silhouette Score**: `0.5483`

This project illustrates that **preprocessing can greatly impact clustering effectiveness**, and the optimal clustering technique depends on both the dataset characteristics and the evaluation metrics used.

---

## 📖 References
- [UCI ML Repository – Wholesale Customers Dataset](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers)
- Scikit-learn Documentation
- Python Data Science Libraries: NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn

---

Feel free to explore and tweak the parameters to see how clustering behavior changes with different settings!

