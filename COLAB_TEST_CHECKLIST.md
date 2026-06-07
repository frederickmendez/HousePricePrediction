# Colab Test Checklist

Do not mark Colab as passed until this has been run in Google Colab.

1. Open Google Colab.
2. Upload `notebooks/house_price_prediction.ipynb`.
3. Upload `data/house_price_50k.csv` into the Colab session.
4. Restart the runtime.
5. Select Runtime -> Run all.
6. Confirm there are no path errors.
7. Confirm all six figures appear.
8. Confirm model metrics:
   - MAE around 15,954
   - RMSE around 19,941
   - R-squared around 99.81%
9. Confirm Tableau exports are created.
10. Download the successfully executed notebook.
11. Open the GitHub Colab link in an incognito/private browser and run all cells again.

GitHub Colab link:

```text
https://colab.research.google.com/github/frederickmendez/HousePricePrediction/blob/main/notebooks/house_price_prediction.ipynb
```

GitHub raw dataset URL:

```text
https://raw.githubusercontent.com/frederickmendez/HousePricePrediction/main/data/house_price_50k.csv
```
