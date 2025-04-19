
# Clustering Assignment

This project compares the performance of different clustering algorithms using various preprocessing techniques and evaluation metrics.

---

## 📊 Dataset
**Iris Dataset** from the UCI Machine Learning Repository.

---

## 🔍 Objective
To evaluate the effectiveness of clustering techniques under different preprocessing scenarios using three evaluation metrics:
- **Silhouette Score**
- **Calinski-Harabasz Index**
- **Davies-Bouldin Index**

---

## 🛠️ Preprocessing Techniques
- No Processing (Raw)
- Normalization (MinMaxScaler)
- Log Transformation
- PCA (2 components)
- Transform + Normalize (T+N)
- Transform + Normalize + PCA (T+N+PCA)

---

## 🤖 Clustering Algorithms
- **K-Means** (k=3,4,5)
- **Hierarchical Clustering** (k=3,4,5)
- **Mean Shift** (automatic cluster detection)

---

## 📈 Evaluation Metrics
| Metric              | Description |
|---------------------|-------------|
| Silhouette Score    | How well samples are clustered |
| Calinski-Harabasz   | Ratio of between-cluster dispersion and within-cluster dispersion |
| Davies-Bouldin      | Lower values indicate better clustering |

---

## ✅ Results Summary

| Algorithm  | Preprocessing     | Clusters | Silhouette | Calinski-Harabasz | Davies-Bouldin |
|------------|-------------------|----------|------------|-------------------|----------------|
| KMeans     | Normalized        | 3        | 0.72       | 4683              | 0.46           |
| Hierarchical | T+N+PCA         | 4        | 0.56       | 3487              | 0.77           |
| Mean Shift | Raw               | Auto     | 0.99       | 5353              | 0.13           |

*Full table available in the notebook.*

---

## 📁 Files
- `clustering_assignment.ipynb`: Colab Notebook with full code and results
- `README.md`: This file

---

## 📌 Conclusion
- **Mean Shift** performed best in the Iris dataset (auto-cluster detection).
- Preprocessing (especially PCA and normalization) greatly impacts cluster performance.
- Silhouette and Davies-Bouldin scores are especially useful for visualizing clustering quality.

---
