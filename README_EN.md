# 🌍 Global Typologies of Democracy (2024)  
**Unsupervised Clustering with V-Dem Data**

🌐 Disponible en [Español](README.md)

![Python](https://img.shields.io/badge/Python-3.10.19-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)
![Model](https://img.shields.io/badge/ML-Unsupervised%20Learning-orange.svg)
![Domain](https://img.shields.io/badge/Field-Political%20Science-purple)

This project identifies **three global types of political regimes in 2024** using unsupervised clustering and the **V-Dem v15** dataset, one of the leading sources for comparative democracy research worldwide.

We combine **PCA** and **K-Means** to group countries based on key democratic dimensions (civil liberties, political equality, participation, etc.).

---

## 🧰 Tech Stack
- **Language:** Python 3.10.19
- **Libraries:**  
  `pandas`, `numpy`, `scikit-learn`,  
  `matplotlib`, `seaborn`, `plotly`, `kaleido`, `pycountry`
- **Data:** V-Dem Country-Year Core Dataset (2024)

---

## 📊 Reproducible Workflow

1️⃣ Indicator selection and normalization  
2️⃣ **PCA** → dimensionality reduction to PC1–PC2  
3️⃣ **Elbow + Silhouette Score** → k = 3  
4️⃣ Model training with **K-Means**  
5️⃣ Institutional interpretation of clusters  
6️⃣ Global visualization (radar + interactive map)  
7️⃣ Export of the labeled dataset ✅

---

## 📈 Main Results

### 🔹 Optimal number of clusters
![Elbow Method](figures/elbow_method.png)

![Silhouette Score](figures/silhouette_score.png)

### 🔹 Democratic profiles (Radar Chart)
![Radar Chart](figures/radar_clusters.png)

### 🔹 PCA Visualization
![PCA Clusters](figures/pca_clusters.png)

---

## 🧠 Resulting Typologies
| Cluster | Interpretation | Predominant Regions |
|--------:|----------------|-------------------|
| 🟢 2 | Consolidated democracies | Western Europe, Oceania, North America, Japan |
| 🟡 0 | Intermediate / hybrid democracies | Latin America, Eastern Europe, North Africa |
| 🔴 1 | Authoritarian regimes | Middle East, Central Asia, Sub-Saharan Africa |

📍 **Argentina** → Cluster 0: electoral democracy with **limitations in political equality and checks on power**, according to V-Dem indicators

---

## 🌐 Interactive World Map

![Map preview](figures/map_preview.png)

🔗 **Online interactive map:**  
https://fernandezelias.github.io/VDem_Democracy_Clustering/figures/democracy_clusters_map.html

---

## 📁 Final Dataset
✔ `data/processed/vdem_clusters_2024.csv`  
Includes: country · PC1–PC2 · final cluster assignment ✅

---

## 🚀 Future work
- Extend to **time series (1990–2024)**
- Test alternative clustering methods: **DBSCAN, Gaussian Mixture Models**
- Compare with external democracy classifications, such as:
  - **Freedom House – Freedom in the World (FiW)**
  - **Economist Intelligence Unit – Democracy Index (EIU)**

These comparisons will help assess the consistency of the model with internationally recognized typologies widely used in Comparative Politics and Political Geography.

---

## ✍️ Author
**Elías Fernández**  
📧 Contact: fernandezelias86@gmail.com  
🔗 LinkedIn: [Profile](https://www.linkedin.com/in/eliasfernandez208)

---

📌 License: **MIT**
