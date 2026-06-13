# ML Practicals

A collection of machine learning projects built while learning. Each practical covers a core ML concept with clean code, visualizations, and documented results.

## Projects

| # | Project | Algorithm | Input | Output |
|---|---------|-----------|-------|--------|
| 01 | [Linear Regression — Weight vs Height](./01-linear-regression-height-weight) | Simple Linear Regression | Weight | Height |
| 02 | [Ridge & Lasso Regression — Predicting FWI](./02-ridge-lasso-regression-algerian-forest-fire/) | Ridge, Lasso | Weather & Fire Indices | FWI |

## Tech Stack

- Python
- Jupyter Notebook
- pandas, numpy, matplotlib, scikit-learn

## Setup

```bash
git clone https://github.com/mohitfr/height-weight-linear-regression.git
cd height-weight-linear-regression
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

## Structure

```
ml-practicals/
├── 01-linear-regression-height-weight/
│   ├── linear_regression.ipynb
│   ├── height-weight.csv
│   ├── height_weight_lr.csv
│   └── README.md
├── 02-ridge-lasso-regression-algerian-forest-fire/
│   ├── ridge_lasso_regression.ipynb
│   ├──data_prep_and_eda.ipynb
│   ├──algerian_forest_fires.csv
│   ├──algerian_forest_fires_cleaned.csv
│   └── README.md
├── .gitignore
└── README.md
```

---
*Adding more practicals as I learn.*