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

MsC Thesis link.: (http://webthesis.biblio.polito.it/id/eprint/33667)

---

## 🎯 Objective

The goal is to identify new tumor phenotypes and potential biomarkers using unsupervised learning techniques, based on clustering tiles from histopathological images using different feature extractors and aggregation methods.

---

## 🔬 Methodology

- Feature extraction from tumor tiles using various extractors 
  - GLCM PyRadiomics
  - MSI prediction
  - Ctranspath
- Dimensionality reduction with:
  - Principal Component Analysis (PCA)
  - Pearson Correlation
- Feature combination across extractors
- Clustering of tumor tiles using the **Bag of Visual Words (BoVW)** technique
  - Phenotype assignment using a **Self-Organizing Map (SOM)**
  - Aggregation of Patients Histogram of tiles **Dendrogram**
- Cluster evaluation using the **Silhouette score**
- Clinical interpretation and validation with an oncologist

---

## 🔄 Project Pipeline

1. **Tile extraction** from histopathological images
    - Tasselization
    - Tumor tissue coordinates detection
2. **Feature extraction** using multiple extractors
    - GLCM (PyRadiomics)
    - MSI prediction model
    - Ctranspath
3. **Dimensionality reduction** (PCA, Pearson)
4. **Visual vocabulary creation** (BoVW)
    - Phenotyping Tumoral tiles with Self-Organizing Map Network 3x3
    - Aggregation of patients by histograms of phenotypes
6. **Cluster evaluation** with Silhouette metric computation
7. **Clinical review** to validate identified clusters and phenotypes

---

## 📁 Project Structure

## Coding References

1. **Colon Tissues Classification in Histopathological image** : [Predicting survival from colorectal cancer histology slides using deep learning: A retrospective multicenter study] (https://journals.plos.org/plosmedicine/article?id=10.1371/journal.pmed.1002730)

2. **Extractors**:

    - GLCM **PyRadiomics**: [Computational Radiomics System to Decode the Radiographic Phenotype] ( https://doi.org/10.1158/0008-5472.CAN-17-0339)
    - **MSI predictor** used as extractor: [Developmaent and interpretation of a pathomic-based model for the prediction of microsatellite instability in  Colorectal Cancer] (https://pmc.ncbi.nlm.nih.gov/articles/PMC7532670/)
    - **Ctranspath**: [Transformer-based unsupervised contrastive learning for histopathological image classification] (https://www.sciencedirect.com/science/article/abs/pii/S1361841522002043)

3. **Stain Normalization Macenko**: [A method for normalizing histology slides for quantitative analysis] (https://ieeexplore.ieee.org/abstract/document/5193250) [Macenko implementation Github Repository] : ()
