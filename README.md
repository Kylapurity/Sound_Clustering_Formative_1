
# Sound Clustering Project

This project explores the use of clustering techniques on unlabeled sound recordings to uncover hidden patterns in audio data. Using Mel-frequency cepstral coefficients (MFCCs) for feature extraction, and dimensionality reduction techniques like PCA and t-SNE, we apply clustering algorithms to group similar audio samples and evaluate the clustering performance.
![image](https://github.com/user-attachments/assets/242b0d6a-b92a-47b4-9ab3-df4aa583e5ae)


---

## Key Features

- **Feature Extraction from Audio Files**  
  Uses MFCCs to convert raw sound into meaningful numerical features for analysis.

- **Visualization of High-Dimensional Data**  
  Utilizes PCA and t-SNE to reduce dimensionality and plot data in 3D for better cluster visualization.

- **Comparison of Clustering Algorithms**  
  K-Means and DBSCAN are implemented and evaluated to identify which better fits the data.

- **Performance Evaluation**  
  Evaluation metrics include **Silhouette Score** and **Davies-Bouldin Index** to determine clustering quality.

- **Real-World Use Case Discussion**  
  Explores how these methods translate to domains like customer segmentation.

---

## Project Structure

```bash
├── purity_kihiu_sound_clustering_assignment.py   # Full implementation code
├── assets/
│   └── clustering_visualizations.png             # PCA and t-SNE visual output
├── README.md
└── 📄 [Attach Your PDF Summary Report Here]
````

---

##  Overview

This project applies clustering techniques to unlabeled sound recordings using:

* **Mel-frequency cepstral coefficients (MFCCs)** for feature extraction
* **PCA** and **t-SNE** for dimensionality reduction
* **K-Means** and **DBSCAN** for clustering
* **Silhouette Score** and **Davies-Bouldin Index** for evaluating clustering quality
* **K Value ** I Used k=3 and this was th result: I ended up picking 4 because I could be able to see more cluster and it had less noise. Where with 3 it had more noise an make the clusters not visible.
     #### K-Means - Silhouette Score: 0.4868, Davies-Bouldin Index: 1.4485
     #### DBSCAN - Silhouette Score: -0.0305, Davies-Bouldin Index: 1.8554
 ####  K = 4 
      #### K-Means - Silhouette Score: 0.4868, Davies-Bouldin Index: 1.4485
      #### DBSCAN - Silhouette Score: -0.0305, Davies-Bouldin Index: 1.8554
---

## Requirements

* Python 3.8+
* Libraries:

  * `librosa`
  * `scikit-learn`
  * `matplotlib`
  * `seaborn`
  * `numpy`
  * `pandas`

---

## 📊 Results Summary

* **Best Dimensionality Reduction:** t-SNE provided better visual separation of clusters compared to PCA.
* **Best Clustering Algorithm:** K-Means outperformed DBSCAN with higher Silhouette Score and lower Davies-Bouldin Index.
* **Optimal Clusters (k):** Identified using the Elbow Method and validated with performance scores.

---
