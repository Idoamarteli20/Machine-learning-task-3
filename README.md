# Machine Learning Assignment 3: Clustering Analysis 🤖

**Author:** Ido Avodi Amterli
**Course:** Introduction to Machine Learning

## 📌 Overview
[cite_start]This repository contains the solution for Assignment 3, focusing on the implementation and comparison of unsupervised learning (clustering) algorithms[cite: 2, 4].
[cite_start]The project involves generating synthetic data, training three different clustering models, optimizing their hyperparameters, and tracking experiments using **MLFlow**[cite: 14].

## 🧠 Algorithms Implemented
[cite_start]The following algorithms were implemented and compared[cite: 4]:
1.  **K-Means:** Centroid-based clustering (Optimized over a range of $k$).
2.  **Agglomerative Clustering:** Hierarchical clustering (Optimized over a range of $k$).
3.  [cite_start]**DBSCAN:** Density-based clustering (Optimized using Grid Search for `eps` and `min_samples`)[cite: 7].

## 📉 Evaluation Metrics
[cite_start]To evaluate the quality of the clusters, the following metrics were used[cite: 15]:
* **Silhouette Score:** The primary metric used to select the "winner" model.
* **WCSS (Within-Cluster Sum of Squares):** Measures cluster compactness.
* **BCSS (Between-Cluster Sum of Squares):** Measures cluster separation.

*(Note: WCSS is calculated for DBSCAN for reporting purposes only, but is not used for optimization as it assumes spherical clusters).*

## 🛠️ Tech Stack & Libraries
* **Python 3.x**
* **Scikit-Learn** (Clustering models & metrics)
* [cite_start]**MLFlow** (Experiment tracking) [cite: 14]
* **Pandas & NumPy** (Data manipulation)
* **Matplotlib & Seaborn** (Visualization)

## 📂 Repository Structure
* `ex3.ipynb` / `main.py`: The main source code containing data generation, training loops, and visualization.
* [cite_start]`Ido_Abodi_Amarteli_Ex3.xlsx`: The final output file containing a summary of all 60+ experiments run[cite: 16].
* `README.md`: Project documentation.

## 🚀 How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YourUsername/RepoName.git](https://github.com/YourUsername/RepoName.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install numpy pandas matplotlib seaborn scikit-learn mlflow
    ```
3.  **Run the notebook/script:**
    Execute the Jupyter Notebook or Python script. The code will:
    * Generate synthetic data.
    * Run optimization loops for all 3 algorithms.
    * Log results to MLFlow.
    * Display comparison charts (Bar plots & 3D Scatter plots).
    * Export the final results to Excel.

## 🏆 Results
The project automatically identifies the best clustering configuration based on the highest Silhouette Score. The final comparison table, including the winner and all experimental data, is saved in the generated Excel file.

---
*Submitted as part of the Machine Learning course requirements.*
