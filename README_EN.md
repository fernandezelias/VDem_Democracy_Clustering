# 🌍 Global Democracy Typologies (2024)  
**Unsupervised clustering using V-Dem data**

![Python](https://img.shields.io/badge/Python-3.11-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)
![Model](https://img.shields.io/badge/ML-Unsupervised%20Learning-orange.svg)

🌐 Also available in Spanish: [README.md](README.md)

This project identifies **three global political regime typologies** in 2024
by applying unsupervised learning techniques to the **V-Dem v15** dataset.

We use **PCA** for dimensionality reduction and **K-Means** to classify countries
based on core democratic attributes.

---

## 🧰 Tech Stack
- **Language:** Python 3.11
- **Libraries:** Pandas, Scikit-learn, Matplotlib, Seaborn, Plotly
- **Dataset:** V-Dem Country-Year Core (2024)

---

## 📊 Workflow

1️⃣ Variable selection + normalization  
2️⃣ **PCA** → PC1 & PC2 as democracy axes  
3️⃣ **Elbow + Silhouette → k = 3**  
4️⃣ **K-Means** clustering  
5️⃣ Cluster interpretation and validation  
6️⃣ Global visualization (radar + map)  
7️⃣ Export of labeled dataset ✅

---

## 📈 Key Findings

### Optimal number of clusters
![Elbow Method](figures/elbow_method.png)

![Silhouette Score](figures/silhouette_score.png)

### Cluster profiles (Radar Chart)
![Radar Chart](figures/radar_clusters.png)

---

## 🧠 Identified regime typologies
| Cluster | Meaning | Main World Regions |
|--------:|---------|------------------|
| 🟢 2 | Full democracies | Western Europe, Oceania, North America, Japan |
| 🟡 0 | Hybrid / transitioning democracies | Latin America, Eastern Europe, North Africa |
| 🔴 1 | Authoritarian regimes | Middle East, Central Asia, Sub-Saharan Africa |

📍 **Argentina** → Cluster 0: intermediate democracy with institutional weaknesses

---

## 🌐 Interactive World Map
📌 Open the interactive version here:  
👉 `figures/democracy_clusters_map.html`

---

## 📁 Output Dataset
✔ `data/processed/vdem_clustering_results.csv`  
Includes: country · PC1-PC2 scores · final cluster assignment ✅

---

## 🚀 Future Work
- **Time-series evolution** of democracy (1990-2024)
- Alternative clustering: **DBSCAN, GMM**
- Triangulation with **external democracy indexes** (FH, EIU, Polity5)

---

## ✍️ Author
**Elías Fernández**  
📧 Email: fernandezelias86@gmail.com  
🔗 LinkedIn: www.linkedin.com/in/eliasfernandez208

---

📌 License: **MIT**