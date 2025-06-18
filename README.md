#  Recipe Flavor Clustering

This project applies **unsupervised learning** techniques to cluster recipes based on their **nutritional profiles** and explores their **ingredient patterns**, **user ratings**, and **similarity-based recommendations**.

---

##  Project Overview

We use the **Food.com Recipes and Reviews** dataset to:

- Standardize and clean nutritional features (calories, fat, protein, etc.)
- Apply **K-Means Clustering** to group similar recipes
- Visualize clusters using **PCA**
- Analyze **average nutritional values**, **ingredient frequency**, and **user ratings** across clusters
- Build a **flavor-based recommendation demo** using intra-cluster similarity

---

## 🗂 Data Source

This project uses publicly available data from Kaggle:

 **Dataset**: [Food.com Recipes and Interactions](https://www.kaggle.com/datasets/kaggle/food-com-recipes-and-user-interactions)

> ⚠ Due to GitHub file size limits, the data files (`recipes.csv`, `reviews.csv`) are **not included** in this repository. Please download them manually from Kaggle and place them in the `/data` folder.

---

## 🧪 Methods Used

-  **Pandas** for data wrangling  
-  **Scikit-learn** for scaling, clustering, and PCA  
-  **Matplotlib / Seaborn** for visualizations  
-  Ingredient frequency extraction via `collections.Counter`  
-  Flavor-based recommendation using Euclidean distance

---

##  Key Insights

- **Cluster 0**: Popular desserts and baked goods (sugar, flour, butter)
- **Cluster 3**: Savory main dishes (garlic, onion, olive oil)
- **Cluster 1 & 2**: Sparse or anomalous recipes (very high calories or missing reviews)
- Ratings and ingredients align well with cluster characteristics

---

## 🎯Demo: Flavor-Based Recommendation

Given a target recipe like _Brownie Heart Cake_, the model recommends similar recipes within its cluster:

| Name                      | Calories | FatContent | ProteinContent |
|---------------------------|----------|------------|----------------|
| Healthy Dhal Soup         | 1127.4   | 27.2       | 67.5           |
| Aloo Ghobi                | 1077.5   | 24.0       | 70.4           |
| My Mom's Shipwreck        | 1102.5   | 20.1       | 72.0           |

---

##  Future Work

- Try GMM or hierarchical clustering for soft boundaries  
- Apply TF-IDF or Word2Vec to ingredient lists  
- Integrate user dietary preferences (e.g., vegan, keto)  
- Build a web app using Streamlit or Dash  
- Conduct cluster validation and silhouette scoring

---

## 🧾 Deliverables

-  Jupyter notebook with full analysis and visualizations  
-  5–10 min video presentation  
-  GitHub repository (this!)

---

##  How to Reproduce

1. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/kaggle/food-com-recipes-and-user-interactions)
2. Place `recipes.csv` and `reviews.csv` inside a `/data` folder
3. Run the Jupyter notebook from top to bottom

---

##  Author

Chitralekha — MSDS @ University of Colorado Boulder  
 Reach out via [GitHub](https://github.com/chitralekha)

---

