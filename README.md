# Penguins Clustering with PCA

This project applies **Principal Component Analysis (PCA)** and **Clustering (Hierarchical and K-Means)** to the famous **Seaborn Penguins dataset**.  

The goal is to analyze physical characteristics of penguins, reduce dimensionality using PCA, and evaluate clustering performance for species and sex classification.

---

## Project Structure
- `trabajo_final_Clustering_JesusNavarro.ipynb` → Jupyter notebook with full implementation.  
- `trabajo_final_Mineria_Clustering_JesusNavarro.docx` → Original project report (in Spanish).  
- `README.md` → Project overview (this file).  
- `requirements.txt` → Python dependencies.  

---

## Key Steps
1. **Data Cleaning**  
   - Remove rows with >50% missing values.  
   - Impute missing `sex` values using a Random Forest Classifier.  

2. **PCA Analysis**  
   - Standardize continuous variables.  
   - Reduce dataset to 3 principal components explaining ~94.5% variance.  
   - Interpret components (body size, sex-related traits, bill dimensions).  

3. **Clustering**  
   - Hierarchical clustering with dendrogram visualization.  
   - K-Means clustering with Elbow and Silhouette methods.  
   - Best result with **5 clusters**, matching species/sex separation.  

---

## Results
- PCA separated **Gentoo penguins** by size (PC1) and **Chinstrap penguins** by bill length (PC3).  
- Clustering correctly distinguished **species and sex groups**, with minor overlap in Adelie/Chinstrap females.  
- Both **hierarchical clustering** and **K-Means** produced consistent results, validated by the **Silhouette Score**.  

---

## Installation
```bash
git clone https://github.com/jd4vid/predictive-modeling-pca-clustering.git
cd penguins-clustering
pip install -r requirements.txt
