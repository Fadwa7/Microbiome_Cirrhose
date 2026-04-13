# Microbiome intestinal & Progression de la Maladie Hépatique

[![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)](https://python.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)](https://scikit-learn.org)
[![SHAP](https://img.shields.io/badge/SHAP-Interpretability-green)](https://shap.readthedocs.io)
[![Dataset](https://img.shields.io/badge/Dataset-MicrobiomeHD-lightgrey)](https://zenodo.org/records/569601)

> **La composition du microbiome intestinal reflète-t-elle la progression de la maladie hépatique, et quelles bactéries sont les biomarqueurs de chaque stade — santé, cirrhose, et encéphalopathie hépatique minimale ?**

---

## 📊 Rapport complet

👉 **[Voir le rapport interactif](https://fadwa7.github.io/microbiome_cirrhose/)**

---

## Stack

`Python 3.10` · `scikit-learn` · `SHAP` · `pandas` · `matplotlib` · `seaborn`

## Résultats clés

- **Balanced Accuracy : 0.644** — ~2× supérieur au hasard (3 classes)
- **MHE** : stade le mieux prédit (recall = 0.81)
- **Veillonella** : biomarqueur principal de la cirrhose (invasion buccale)
- **Faecalibacterium** : effondrement progressif vers l'encéphalopathie (×3 dans SHAP MHE)

## Reproduire

```bash
conda create -n microbiome python=3.10
conda activate microbiome
pip install pandas numpy matplotlib seaborn scikit-learn shap requests jupyter
jupyter notebook notebooks/01_data_loading.ipynb
```

> Le dataset est téléchargé automatiquement depuis Zenodo au lancement.

---

*Fadwa El Khaddar — Ingénieure Bioinformatique · Voir aussi : [TCGA-COAD Multiomics MOFA+](https://fadwa7.github.io/TCGA_COAD_multiomics/)*
