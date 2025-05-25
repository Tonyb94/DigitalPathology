<h2 align="center">🧬 Comparison by Clustering of Feature Extractors from Colorectal Tumor Histopathology Tiles Aggregated with Bag of Visual Words</h2>

<p align="center">
  <img src="https://github.com/Tonyb94/DigitalPathology/blob/master/PIPELINE.jpeg" height="400" alt="Project Pipeline" />
</p>

---

## 📝 Project Description

Colorectal cancer (CRC) is the third most common type of cancer and the third leading cause of cancer-related death worldwide. This study aims to analyze and extract potential morphological biomarkers from histopathological images of surgically resected colorectal tumors from two subject groups:

- **IANG group**: patients under 40 years old (9 patients)
- **OLD group**: patients over 40 years old (8 patients)

These ultra-high-resolution images (83456 × 185600 pixels) were stained with Hematoxylin and Eosin (H&E) and acquired using a Mirax scanner at Niguarda Hospital in Milan.

---

## 🎯 Objective

The goal is to identify new tumor phenotypes and potential biomarkers using unsupervised learning techniques, based on clustering tiles from histopathological images using different feature extractors and aggregation methods.

---

## 🔬 Methodology

- Feature extraction from tumor tiles using various extractors
- Dimensionality reduction with:
  - Principal Component Analysis (PCA)
  - Pearson Correlation
- Feature combination across extractors
- Clustering of tumor tiles using the **Bag of Visual Words (BoVW)** technique
- Phenotype assignment using a **Self-Organizing Map (SOM)**
- Cluster evaluation using the **Silhouette score**
- Clinical interpretation and validation with an oncologist

---

## 🔄 Project Pipeline

1. **Tile extraction** from histopathological images
2. **Feature extraction** using multiple extractors
3. **Dimensionality reduction** (PCA, Pearson)
4. **Visual vocabulary creation** (BoVW)
5. **Clustering with Self-Organizing Map**
6. **Cluster evaluation** with Silhouette metric
7. **Clinical review** to validate identified clusters and phenotypes

---

## 📁 Project Structure

