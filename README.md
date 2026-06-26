# Data Analysis of Public Procurement Data

This is an internship project for the **Big Data Analysis** specialization.
The project covers the full data analytics cycle: from raw data profiling and ETL processing to statistical analysis and a trained predictive machine learning model.

## Project Overview

The project is based on company-provided public procurement data.
The main goal was to analyze factors influencing tender outcomes and build a model that predicts whether a supplier's bid is likely to win a tender.

## Project Structure

```text
.
├── notebooks/
│   ├── Week1_профилирование_данных.ipynb   # Data profiling
│   ├── Week2_ETL_очистка_данных.ipynb      # ETL and data cleaning
│   ├── Week3_анализ_и_модель.ipynb         # EDA, statistics, and modeling
│   └── Week4_финализация.ipynb             # Finalization and documentation
├── data/                                    # Data files are not included in the repository
├── models/
│   └── tender_model.joblib                  # Serialized trained model
├── figures/                                 # Generated charts and figures
├── requirements.txt
└── README.md
```

## Technologies Used

* **Python 3**, pandas, NumPy — data processing and analysis
* **scikit-learn** — machine learning models, evaluation, and cross-validation
* **Matplotlib, Seaborn** — data visualization
* **SciPy** — statistical hypothesis testing
* **joblib** — model serialization
* **Jupyter Notebook** — development, documentation, and reproducible analysis
* **Git/GitHub** — version control and project publication

## Main Results

* Built a predictive model for tender bid outcomes.
* Selected **Gradient Boosting** as the final model.
* Achieved **ROC-AUC ≈ 0.98**, stable under 5-fold cross-validation.
* Identified the most important factor: **price rank within a lot**.
* Confirmed the statistical importance of price-related factors using hypothesis testing.
* Created a reproducible project structure with notebooks, figures, a saved model, and documentation.

## Data Availability

The raw CSV files are **not included** in this repository due to privacy considerations.
The original datasets may contain sensitive supplier-related information, so they are excluded from public access.

The repository includes executed notebooks, generated figures, the trained model, `requirements.txt`, and documentation as evidence of the completed work.

Full ETL re-execution is possible only for authorized users who have access to the original private CSV files. To re-run the ETL notebook, place the original files in the expected local folder:

```text
data/raw/
```

Expected raw files:

```text
data/raw/suppliers.csv
data/raw/kraska.csv
```

## Reproduction

Install the required packages:

```bash
pip install -r requirements.txt
```

Open Jupyter Notebook:

```bash
jupyter notebook
```

Run the notebooks sequentially:

```text
Week1 → Week2 → Week3 → Week4
```

Note: full reproduction from raw data requires access to the original CSV files. Without the raw files, the executed notebooks, figures, saved model, and documented outputs still demonstrate the completed analysis.

## Author

Amankos Danial Dauletuly,
Big Data Analysis student,
Astana IT University,
Industrial Practice, 2026.
