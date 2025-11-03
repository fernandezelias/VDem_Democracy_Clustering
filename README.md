# 🌍 Tipologías Globales de Democracia (2024)  
**Clustering no supervisado con datos V-Dem**

![Python](https://img.shields.io/badge/Python-3.11-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)
![Model](https://img.shields.io/badge/ML-Unsupervised%20Learning-orange.svg)

🌐 Disponible también en inglés: [README_EN.md](README_EN.md)

Este proyecto identifica **tres tipos globales de regímenes políticos en 2024**
utilizando clustering no supervisado y datos del prestigioso dataset **V-Dem v15**.

Se combinan técnicas de **PCA** y **K-Means** para agrupar países según dimensiones
democráticas clave (libertades civiles, igualdad política, participación, etc.).

---

## 🧰 Stack Tecnológico
- **Lenguaje:** Python 3.11
- **Librerías:** Pandas, Scikit-learn, Matplotlib, Seaborn, Plotly
- **Data:** V-Dem Country-Year Core Dataset (2024)

---

## 📊 Flujo de trabajo reproducible

1️⃣ Selección y normalización de indicadores democráticos  
2️⃣ **PCA** → reducción de 5 dimensiones a PC1-PC2  
3️⃣ **Elbow + Silhouette Score → k = 3**  
4️⃣ Entrenamiento del modelo **K-Means**  
5️⃣ Interpretación institucional de clusters  
6️⃣ Visualización global (radar + mapa interactivo)  
7️⃣ Exportación del dataset etiquetado ✅

---

## 📈 Resultados principales

### 🔹 Validación del número óptimo de clusters
![Elbow Method](figures/elbow_method.png)

![Silhouette Score](figures/silhouette_score.png)

### 🔹 Perfiles democráticos (Radar Chart)
![Radar Chart](figures/radar_clusters.png)

---

## 🧠 Tipologías resultantes
| Cluster | Interpretación | Regiones predominantes |
|--------:|----------------|----------------------|
| 🟢 2 | Democracias consolidadas | Europa Occidental, Oceanía, Norteamérica, Japón |
| 🟡 0 | Democracias intermedias / híbridas | América Latina, Europa del Este, Norte de África |
| 🔴 1 | Regímenes autoritarios | Medio Oriente, Asia Central, África Subsahariana |

📍 **Argentina** → Cluster 0: democracia intermedia con tensiones institucionales

---

## 🌐 Mapa Mundo Interactivo
📌 *Explora país por país:*  
👉 `figures/democracy_clusters_map.html`

---

## 📁 Datos finales
✔ `data/processed/vdem_clustering_results.csv`  
Incluye: país · PC1-PC2 · asignación final de cluster ✅

---

## 🚀 Próximos pasos
- Extender análisis a **series temporales (1990-2024)**
- Probar modelos alternativos: **DBSCAN, Gaussian Mixture Models**
- Comparar con clasificaciones externas (Freedom House, EIU, Polity5)

---

## ✍️ Autor
**Elías Fernández**  
📧 Contacto: fernandezelias86@gmail.com  
🔗 LinkedIn: www.linkedin.com/in/eliasfernandez208

---

📌 Licencia: **MIT**