
# 🧠 Data-Driven Subtyping of Alzheimer’s Disease ED Presentations via Unsupervised Machine Learning

This repository contains the full analysis pipeline and source code used in the study:

**"Data-Driven Subtyping of Alzheimer’s Disease ED Presentations via Unsupervised Machine Learning"**

> Alkam T., et al. (2025) — *Manuscript under review*

---

## 📘 Overview

This project investigates the complex landscape of emergency department (ED) presentations among older adults with Alzheimer’s disease (AD) using a data-driven unsupervised machine learning pipeline. Leveraging the 2022 Nationwide Emergency Department Sample (NEDS)—the largest all-payer ED dataset in the U.S.—we identified age-stratified multimorbidity clusters based on the 30 most prevalent ICD-10 diagnosis codes in each age group (60–64, 65–74, 75–84, 85+).

We applied Uniform Manifold Approximation and Projection (UMAP) for dimensionality reduction and Hierarchical Density-Based Spatial Clustering of Applications with Noise (HDBSCAN) for density-aware clustering. The resulting clusters were visualized and interpreted using annotated diagnosis heatmaps, revealing distinct and clinically meaningful subtypes.

These clusters highlight evolving comorbidity themes across the aging continuum, including:

Psychiatric–metabolic overlap in younger-old adults

Cardiorenal syndromes and frailty trajectories in mid- to late-old age

Terminal multimorbidity and end-of-life care patterns in the oldest-old

This repository contains the full reproducible pipeline, including data preprocessing, clustering, heatmap construction, and cluster interpretation notebooks.

Our work aims to support precision emergency medicine, inform risk stratification models, and enable more personalized care strategies for patients with AD in acute settings.

---

## 🧪 Methods

This repository includes the full implementation of the pipeline:

### 🔁 Analysis Pipeline

1. **Data Preparation**

   * Preprocessing of NEDS data by age group (60–64, 65–74, 75–84, ≥85)
   * Binary matrix creation using top 30 ICD-10 diagnosis codes

2. **Dimensionality Reduction**

   * UMAP projection of binary comorbidity vectors

3. **Unsupervised Clustering**

   * HDBSCAN clustering within each age group

4. **Heatmap Construction**

   * Calculation of cluster-wise comorbidity loadings
   * Annotated heatmaps for clinical interpretation

5. **Labeling and Thematic Profiling**

   * Diagnosis codes with loading ≥0.40 retained
   * Clinical themes derived per cluster

---

## 📁 Files

* `Final_!_NEDS_2022_Agegroups_Top30.ipynb`: Main analysis notebook containing all code for:

  * UMAP-HDBSCAN clustering
  * Cluster profiling
  * Heatmap generation
  * Export of labeled comorbidity themes

* `README.md`: Overview and usage guide

---

## 📊 Requirements

This notebook uses the following packages:

```bash
Python >= 3.8

pip install:
- pandas
- numpy
- matplotlib
- seaborn
- umap-learn
- hdbscan
- scikit-learn
```

---

## ▶️ How to Run

```bash
# Clone the repository
git clone https://github.com/your-username/AD_ED_Subtyping.git
cd AD_ED_Subtyping

# Open the Jupyter notebook
jupyter notebook Data-Driven Subtyping of Alzheimer’s Disease ED Presentations via Unsupervised Machine Learning.ipynb
```

Data from HCUP’s NEDS 2022 must be accessed separately due to licensing restrictions.

---

## 📈 Example Output

The notebook will generate:

* Cluster-labeled UMAP plots
* Annotated heatmaps per age group
* Tables summarizing top comorbidities and cluster themes

---

## 📜 Citation

If you use this code, please cite our paper (preprint pending, add DOI once available):

```
Alkam T., et al. (2025). Data-Driven Subtyping of Alzheimer’s Disease ED Presentations via Unsupervised Machine Learning.
```

---

## 📧 Contact

For questions or collaboration inquiries, contact:
**Tursun Alkam, MD, PhD, MBA**
Email: [YourEmailHere]

---

Would you like me to export this as a `README.md` file for you to upload directly to GitHub?
