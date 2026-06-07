# House Price Prediction

This project predicts house prices using a public Kaggle dataset and a supervised regression workflow. The aim is practical: give a property analyst a consistent first estimate, then explain the main drivers behind that estimate.

## Dataset

The dataset is `house_price_50k.csv` from Kaggle:

https://www.kaggle.com/datasets/miadul/house-price-prediction-dataset

The dataset contains 50,000 rows and 19 columns. The target variable is `price`. The Kaggle metadata lists the licence as Apache 2.0. The public source does not prove country, currency, transaction date or official market provenance, so the notebook uses `price units` rather than inventing a currency.

## Objectives

- Load and inspect the house-price dataset.
- Prepare numeric and categorical features.
- Train Linear Regression, Ridge Regression and Random Forest models.
- Compare MAE, RMSE, R-squared and cross-validation results.
- Export six final figures and Tableau-ready CSV files.

## Repository Structure

```text
HousePricePrediction/
- .gitignore
- COLAB_TEST_CHECKLIST.md
- data/
    - house_price_50k.csv
    - README.md
- evidence/
    - local_notebook_execution_log.md
- figures/
    - figure_01_price_distribution.png
    - figure_02_location_income_price.png
    - figure_03_price_vs_area.png
    - figure_04_correlation_heatmap.png
    - figure_05_actual_vs_predicted.png
    - figure_06_feature_importance.png
- notebooks/
    - house_price_prediction.ipynb
- README.md
- requirements.txt
- tableau-pack/
    - cleaned_house_price_50k.csv
    - feature_importance.csv
    - model_metrics.csv
    - model_predictions.csv
    - numeric_correlations_with_price.csv
    - summary_by_location.csv
    - summary_by_location_income.csv
    - tableau_dashboard_build_note.md
```

## Final Results

Best model: Ridge Regression

- MAE: 15,954 price units
- RMSE: 19,941 price units
- R-squared: 99.81%
- Cross-validation RMSE: 20,018 price units

The main business insight is simple: area is the strongest driver of price in this dataset. Location and income level add market context, while the other property and neighbourhood fields refine the estimate.

## Installation

```bash
pip install -r requirements.txt
```

## Local Execution

Open `notebooks/house_price_prediction.ipynb` and run all cells from a clean kernel. The notebook first looks for:

```text
data/house_price_50k.csv
```

It writes figures to `figures/` and Tableau files to `tableau-pack/`.

## Google Colab

Colab badge placeholder: TODO: add Colab URL after GitHub publication

Before the GitHub repository exists, upload both:

- `notebooks/house_price_prediction.ipynb`
- `data/house_price_50k.csv`

After GitHub publication, replace the notebook's `GITHUB_RAW_DATA_URL` placeholder with the raw dataset URL.

## Tableau Files

The `tableau-pack/` folder contains cleaned data, predictions, model metrics, feature importance and summary CSV files. A real Tableau workbook is not included because no `.twbx` file exists yet.

## Limitations

The model is accurate on this dataset, but it should not be treated as a live valuation engine. A production version would need verified transaction data, exact location, transaction dates, property condition and market indicators.

## Academic Purpose

This repository supports an academic machine learning and visualisation assessment. It is designed for reproducibility and review, not commercial deployment.

## Links

- GitHub repository: TODO: add GitHub repository URL after publication
- Google Colab notebook: TODO: add Colab URL after GitHub publication
