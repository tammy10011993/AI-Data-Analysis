
# 🧠 K-Means Customer Segmentation – Wholesale Dataset

This project applies **K-Means Clustering** to segment wholesale customers based on their annual spending behavior across multiple product categories. The objective is to uncover patterns that can drive data-informed business decisions, such as personalized promotions, product bundling, and region-based logistics planning.

---

## 📂 Dataset Overview

The dataset comes from the UCI Machine Learning Repository and includes:

- Annual spending in units (Fresh, Milk, Grocery, Frozen, Detergents_Paper, Delicassen)
- Categorical features: `Channel` (1 = Horeca, 2 = Retail) and `Region` (1 = Lisbon, 2 = Oporto, 3 = Other)

---

## 🧪 Project Steps

1. **Data Exploration & Cleaning**
2. **Feature Scaling using StandardScaler**
3. **K-Means Clustering**
   - Elbow Method to determine optimal K
   - Silhouette Score to evaluate cluster quality
4. **Dimensionality Reduction using PCA**
5. **Cluster Visualization**
6. **Cluster Profiling**
   - Average spending per category per cluster
   - Channel and region composition
7. **Business Insights & Strategy**
   - Targeted promotions
   - Product bundling suggestions
   - Region-wise logistics planning

---

## 📊 Visualizations

- Elbow Method plot
- Silhouette Score (optional)
- Cluster scatterplot (PCA)
- Heatmap of cluster profiles
- Cluster × Channel and Cluster × Region stacked bar plots

---

## 🧠 Key Insights

- Some clusters are high in Fresh & Milk (likely Horeca)
- Others are Retail-dominant with high Grocery and Frozen
- Region overlays showed majority of customers in "Other" areas
- Segment-specific strategies help optimize promotions and inventory

---

## 🛠 Tools Used

- Python (Jupyter Notebook)
- pandas, numpy
- matplotlib, seaborn, plotly (for visualization)
- scikit-learn (StandardScaler, KMeans, PCA)
- Tableau (for dashboard visualization – optional)
- VS Code (with GitHub Copilot & Data Wrangler)

---

## ✅ Folder Contents

| File                          | Description                                |
|-------------------------------|--------------------------------------------|
| `KMeans_Clustering_Cleaned.ipynb` | Final annotated notebook                   |
| `Wholesale customers data.csv`    | Dataset used                               |
| `images/` (optional)              | Saved plots and visualizations             |

---

## 📢 Author

Tamanna Atiq  
*AI Engineer in training | Data-driven storyteller | Driven by insights that matter*

---

## 📎 License

This project is open-source under the [MIT License](LICENSE).
