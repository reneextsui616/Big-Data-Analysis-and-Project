### Replication Guide

Requirements
- Python 3.9+
- Packages: pandas, numpy, matplotlib, seaborn, scikit-learn, imbalanced-learn

Install
```bash
pip install -U pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
```

Data
- Ensure `Bank_Marketing_Ready_to_TRAIN_MODEL.csv` is available at the path referenced in the notebook. If needed, update the path in the first data-loading cell of `bank_marketing_analysis.ipynb`.

Run
1. Open the Jupyter Notebook: 
```bash
jupyter notebook bank_marketing_analysis.ipynb
```
2. Run all cells. Key sections:
   - EDA and target distribution
   - KMeans clustering + PCA visualization
   - Modeling (LR/DT/RF) with PCA and tuning
   - Recall-optimized RF using SMOTE (ROC, confusion matrix)
   - ROI and prescriptive actions

Export Figures
- From notebook cells generating plots, save to `figures/` as PNG for inclusion in the report.
```bash
plt.savefig("figures/pca_clusters.png", dpi=300, bbox_inches="tight")
```


