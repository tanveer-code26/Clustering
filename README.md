# Clustering Analysis

## Overview
This project presents a comparative analysis of different clustering algorithms applied to the **Wholesale Customers Data** from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/machine-learning-databases/00292/Wholesale%20customers%20data.csv). The clustering techniques evaluated include:

- **K-Means Clustering**
- **Hierarchical Clustering**
- **Mean-Shift Clustering**

Various preprocessing methods were explored to assess their impact on clustering performance:

- No Preprocessing
- Normalization
- Power Transformation
- PCA (Principal Component Analysis)

## Dataset
The dataset contains features representing annual spending in monetary units on diverse product categories:

- Fresh
- Milk
- Grocery
- Frozen
- Detergents_Paper
- Delicassen

## Implementation
### Preprocessing Techniques:
- **Standard Scaling**: Scales features to have zero mean and unit variance.
- **Power Transformation**: Makes data more Gaussian-like to stabilize variance and minimize skewness.
- **PCA (Principal Component Analysis)**: Reduces data dimensions while retaining maximum variance.

### Evaluation Metrics:
Clustering performance is assessed using the following metrics:

1. **Silhouette Score** – Indicates how well data points fit within their assigned cluster.
2. **Calinski-Harabasz Score** – Evaluates cluster separation by comparing between- and within-cluster dispersion.
3. **Davies-Bouldin Score** – Measures cluster similarity; lower values indicate better-defined clusters.

### Outputs:
Results are generated and saved in images folder as:

- **`clustering_results.csv`** – Contains scores from each algorithm-preprocessing combination.
- **Cluster Visualizations** – Includes visual output for each algorithm (e.g., `K-Means_clusters.png`, `Hierarchical_clusters.png`, `Mean-Shift_clusters.png`).
- **Dendrogram** – Hierarchical clustering dendrogram saved as `dendrogram.png`.
- **Performance Comparison Table** – A consolidated view of all evaluation scores.

### Sample Visualizations:

#### K-Means Clustering
![K-Means_clusters](https://github.com/user-attachments/assets/545fac4a-9686-4f20-b954-ec9185f344c0)

#### Hierarchical Clustering Dendrogram
![dendrogram](https://github.com/user-attachments/assets/bc4fa015-6dc9-43d0-9b2f-a1655a8b17d7)


## Conclusion
This project offers insights into how different clustering algorithms behave under various preprocessing techniques. The optimal clustering approach may vary depending on the evaluation metric and the structure of the dataset.
