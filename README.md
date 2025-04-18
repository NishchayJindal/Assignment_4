# Clustering Analysis on Preprocessed Data

This project applies **K-Means**, **Mean-Shift**, and **Hierarchical Clustering** to a dataset, comparing the performance of each method using standard clustering evaluation metrics. It also visualizes the results via heatmaps and summary tables.

---

## 🧠 Methods Used

- **K-Means Clustering**
- **Mean-Shift Clustering**
- **Hierarchical Clustering**

---

## ⚙️ Preprocessing Techniques

The following preprocessing strategies were tested to evaluate their effect on clustering quality:

- Raw Data (No Preprocessing)
- Normalization
- Standardization
- Principal Component Analysis (PCA)

---

## 📏 Evaluation Metrics

Each clustering output was evaluated with:

- **Silhouette Score**  
  Measures how similar an object is to its own cluster compared to other clusters.
  
- **Calinski-Harabasz Index**  
  Higher values indicate better defined clusters.
  
- **Davies-Bouldin Index**  
  Lower values indicate better clustering (compact and well-separated clusters).

---

## 💡 Results Summary

- PCA preprocessing consistently improves clustering quality.
- **Mean-Shift** achieved the highest **Silhouette Score** (`0.710`) with PCA.
- **K-Means** performed competitively on both **Calinski-Harabasz** and **Davies-Bouldin**.
- **Hierarchical Clustering** was stable and effective when combined with PCA.

Refer to the `heatmap_*.png` and `table_*.png` files for detailed metric comparisons.

---

## 🖼️ Visualizations

The following heatmaps and tables were generated for analysis:

| Visualization            | Description                          |
|---------------------------|--------------------------------------|
| `heatmap_kmeans.png`      | Heatmap of K-Means performance       |
| `heatmap_meanshift.png`   | Heatmap of Mean-Shift performance    |
| `heatmap_hierarchical.png`| Heatmap of Hierarchical performance  |
| `table_kmeans.png`        | Metric table for K-Means            |
| `table_meanshift.png`     | Metric table for Mean-Shift         |
| `table_hierarchical.png`  | Metric table for Hierarchical       |

---

## 💻 Usage

1. Install dependencies:
    ```bash
    pip install numpy pandas scikit-learn matplotlib seaborn
    ```

2. Run the analysis:
    ```bash
    python clustering_analysis.py
    ```

3. Results will be saved as `.png` files for both tables and heatmaps.

---

## 📌 Conclusion

This project highlights the importance of preprocessing, especially **PCA**, in improving clustering performance. Mean-Shift with PCA delivered the best separation, while K-Means and Hierarchical Clustering provided solid and interpretable structures when the data was appropriately reduced.

---

## 📁 File Structure

