# 🧬 Gene Expression Analysis of Wolfram Syndrome using RNA-Seq Data

## 📌 Project Overview

This project presents a comprehensive **bioinformatics pipeline** for analyzing gene expression patterns in **Wolfram Syndrome**, a rare neurodegenerative disorder caused by mutations in the **WFS1 gene**.

Using publicly available **RNA-Seq datasets (GSE212256)**, this study identifies:

* Differentially expressed genes (DEGs)
* Key biological pathways
* Potential biomarkers
* Machine learning-based classification of disease vs control

---

## 🎯 Objectives

* Analyze transcriptomic changes caused by WFS1 mutation
* Identify significant **upregulated and downregulated genes**
* Perform **cross-dataset validation**
* Apply **machine learning models** for classification
* Propose a novel metric: **Transcriptomic Dysregulation Index (TDI)**
* Discover a **robust biomarker gene panel**

---

## 📊 Dataset Information

**Source:** NCBI GEO
**Accession ID:** GSE212256

### Dataset 1:

* File: `GSE212256_W024deW121.csv`
* Genes: 10,081
* Condition: Standard differentiation

### Dataset 2:

* File: `GSE212256_W024amxDEW121amx.csv`
* Genes: 9,914
* Condition: Amyloid-treated

### Key Features:

* `p_val` → statistical significance
* `avg_logFC` → log2 fold change
* `pct.1`, `pct.2` → expression percentages
* `p_val_adj` → adjusted p-value

---

## ⚙️ Technologies & Tools Used

* **Python 3.10+**
* **Google Colab**
* pandas, numpy
* matplotlib, seaborn
* scikit-learn
* scipy
* networkx

---

## 🔬 Methodology

The project follows a structured pipeline:

1. **Data Loading & Preprocessing**
2. **Differential Gene Expression (DEG) Analysis**
3. **Visualization**

   * Volcano Plot
   * Heatmap
   * Bar plots
4. **Dimensionality Reduction**

   * PCA
   * t-SNE
5. **Pathway Analysis**
6. **Machine Learning Classification**

   * Logistic Regression
   * Random Forest
   * SVM
   * Gradient Boosting
7. **Biomarker Discovery**

   * Cross-dataset concordance
   * Feature importance
   * TDI scoring

---

## 🧠 Key Results

* ✔ Identified:

  * **23 upregulated genes**
  * **9 downregulated genes**
* ✔ Strong dataset correlation: **r = 0.806**
* ✔ ML Models achieved:

  * **Accuracy = 100%**
  * **AUC = 1.000**
* ✔ Mitochondrial genes (MT-ND family) highly upregulated
* ✔ Beta-cell function genes significantly downregulated
* ✔ Final **5-gene biomarker panel** identified

---

## 📈 Important Outputs

* Volcano plots (DEG visualization)
* Heatmaps (gene expression patterns)
* PCA & t-SNE plots (sample separation)
* ROC curves (ML performance)
* Feature importance graphs
* Pathway analysis plots

(All outputs available in `/outputs` folder)

---

## 💡 Novel Contribution

### 🧪 Transcriptomic Dysregulation Index (TDI)

A new composite metric combining:

* Fold change magnitude
* Statistical significance
* Cross-dataset consistency
* Variance contribution

Used to rank genes for **biomarker discovery**

---

## 📁 Repository Structure

```
📦 wolfram-syndrome-rnaseq-analysis
 ┣ 📜 Wolfram_Syndrome_RNASeq_Extended.ipynb
 ┣ 📊 GSE212256_W024deW121.csv
 ┣ 📊 GSE212256_W024amxDEW121amx.csv
 ┣ 📁 outputs/
 ┃ ┣ volcano_plots.png
 ┃ ┣ heatmaps.png
 ┃ ┣ PCA.png
 ┃ ┣ tsne.png
 ┃ ┣ ROC_curves.png
 ┃ ┗ feature_importance.png
 ┗ 📄 README.md
```



## 👨‍💻 Authors

* **Dheepakraj S** – 22MIA1127
* **S Saran Karthik** – 22MIA1001

M.Tech Business Analytics
VIT Chennai

---

## 📚 References

* Kitamura et al., 2022 – GSE212256 Dataset
* Esteban-Bueno et al., 2025
* Frontino et al., 2025
* Additional references included in project report

---

## 🚀 Future Scope

* Validation using real patient datasets
* Integration with proteomics & genomics
* Drug target identification
* Clinical biomarker validation

---
