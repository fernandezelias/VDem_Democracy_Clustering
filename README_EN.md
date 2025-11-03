# 🌍 Global Democracy Typologies (2024)  
**Unsupervised clustering with V-Dem data**

![Python](https://img.shields.io/badge/Python-3.10.19-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)
![Model](https://img.shields.io/badge/ML-Unsupervised%20Learning-orange.svg)

🌐 Disponible en español: [README.md](README.md)

This project identifies **three global types of political regimes in 2024**
using unsupervised clustering and the prestigious **V-Dem v15** dataset.

It combines **PCA** and **K-Means** techniques to group countries based on key
democratic dimensions (civil liberties, political equality, participation, etc.).

---

## 🧰 Technology Stack
- **Language:** Python 3.10.19
- **Libraries:**  
  `pandas`, `numpy`, `scikit-learn`,  
  `matplotlib`, `seaborn`, `plotly`, `kaleido`, `pycountry`
- **Data Source:** V-Dem Country-Year Core Dataset (2024)

---

## 📊 Reproducible Workflow

1️⃣ Democratic indicator selection and normalization  
2️⃣ **PCA** → dimensionality reduction to PC1–PC2  
3️⃣ **Elbow + Silhouette Score** → k = 3  
4️⃣ K-Means clustering  
5️⃣ Institutional interpretation of clusters  
6️⃣ Global visualization (radar + interactive map)  
7️⃣ Labelled dataset export ✅

---

## 📈 Key Results

### 🔹 Optimal cluster validation
![Elbow Method](figures/elbow_method.png)

![Silhouette Score](figures/silhouette_score.png)

### 🔹 Democratic profile comparison (Radar Chart)
![Radar Chart](figures/radar_clusters.png)

### 🔹 PCA Visualization
![PCA Clusters](figures/pca_clusters.png)

---

## 🧠 Cluster Typologies

| Cluster | Interpretation | Main regions |
|--------:|----------------|--------------|
| 🟢 2 | Consolidated democracies | Western Europe, Oceania, North America, Japan |
| 🟡 0 | Intermediate / hybrid democracies | Latin America, Eastern Europe, North Africa |
| 🔴 1 | Authoritarian regimes | Middle East, Central Asia, Sub-Saharan Africa |

📍 **Argentina** → Cluster 0: intermediate democracy with institutional tensions

---

## 🌐 Interactive World Map

![Map preview](figures/map_preview.png)

📌 Explore country by country:  
🔗 **Interactive map:** [democracy_clusters_map.html](figures/democracy_clusters_map.html)

> If GitHub does not render the HTML preview, download and open locally.

---

## 📁 Final Dataset

✔ `data/processed/vdem_clusters_2024.csv`  
Includes: country · PC1–PC2 · final cluster assignment ✅

---

## 🚀 Future Work
- Extend analysis to **time series (1990–2024)**
- Test alternative models: **DBSCAN, Gaussian Mixture Models**
- Compare against external classifications (Freedom House, EIU, Polity5)

---

## ✍️ Author
**Elías Fernández**  
📧 Contact: fernandezelias86@gmail.com  
🔗 LinkedIn: www.linkedin.com/in/eliasfernandez208

---

📌 License: **MIT**