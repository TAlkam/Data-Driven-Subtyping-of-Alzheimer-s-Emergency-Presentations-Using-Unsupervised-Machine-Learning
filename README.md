
# 🧠 Data-Driven Subtyping of Alzheimer’s Disease ED Presentations via Unsupervised Machine Learning

This repository contains the full analysis pipeline and source code used in the study:

**"Data-Driven Subtyping of Alzheimer’s Disease ED Presentations via Unsupervised Machine Learning"**

> Alkam T., et al. (2025) — *Manuscript under review*

---

## 📘 Overview

Older adults with Alzheimer's disease (AD) often present to emergency departments (EDs) with complex, overlapping comorbidities. In this study, we applied an **unsupervised machine learning pipeline** to the 2022 Nationwide Emergency Department Sample (NEDS) to identify age-stratified multimorbidity clusters based on the top 30 most common ICD-10 diagnoses.

Using **UMAP for dimensionality reduction** and **HDBSCAN for density-based clustering**, we identified clinically meaningful subtypes that reflect evolving patterns of psychiatric, cardiometabolic, infectious, and palliative care burden across the aging continuum.

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
