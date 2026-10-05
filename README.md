# Cervical-Cancer Risk Classification

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![Task](https://img.shields.io/badge/task-classification-4a4a52?style=flat-square)

Supervised machine-learning classification of **cervical-cancer risk** from the Kaggle
[Cervical Cancer Risk Factors](https://www.kaggle.com/datasets/loveall/cervical-cancer-risk-classification)
dataset (UCI). The data mixes demographics, sexual/medical history, and diagnostic test results
(Hinselmann, Schiller, cytology, biopsy) — the kind of messy clinical table that needs real
cleaning before any model will behave.

## What's inside

| File | Role |
|------|------|
| `cervical-cancer-classification.ipynb` | Full notebook: cleaning → EDA → feature prep → modelling → evaluation |
| `kag_risk_factors_cervical_cancer.csv` | The raw risk-factors dataset |

## Pipeline

1. **Clean** — the raw file encodes missing values as `?`; coerce to numeric, impute, and drop uninformative columns.
2. **Explore** — class balance, feature distributions, and correlation with the target.
3. **Model** — train and compare classifiers on the risk features, with attention to the heavy class imbalance.
4. **Evaluate** — accuracy alongside precision / recall / ROC-AUC, since a false negative matters far more than a false positive here.

## Run it

```bash
pip install scikit-learn pandas numpy matplotlib seaborn
jupyter notebook cervical-cancer-classification.ipynb
```

> Learning / research project on public data — not a diagnostic tool. See the notebook for the models compared and their measured scores.
