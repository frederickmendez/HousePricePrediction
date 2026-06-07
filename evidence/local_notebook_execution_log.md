# Local Notebook Execution Log

Status: PASS

```text
## Cell 4
Project root: C:\Users\frede\OneDrive\Documentos\Chicken Project\HousePricePrediction
Dataset path: C:\Users\frede\OneDrive\Documentos\Chicken Project\HousePricePrediction\data\house_price_50k.csv
## Cell 6
## Cell 8
Loaded dataset with shape: (50000, 19)
   area  bedrooms  bathrooms  ...  location  income_level         price
0  1360         6          2  ...   premium           low  5.952493e+05
1  4272         5          2  ...       low           low  1.571208e+06
2  3592         1          4  ...   premium           mid  1.379943e+06
3   966         5          2  ...    medium           low  4.367819e+05
4  4926         4          3  ...       low           mid  1.792425e+06

[5 rows x 19 columns]
## Cell 10
Rows: 50000
Columns: 19
area                      int64
bedrooms                  int64
bathrooms                 int64
floors                    int64
age                       int64
distance                  int64
garage                    int64
parking                   int64
garden                    int64
security                  int64
school_nearby             int64
hospital_nearby           int64
shopping_mall_nearby      int64
public_transport          int64
crime_rate              float64
population_density        int64
location                    str
income_level                str
price                   float64
dtype: object
## Cell 12
Missing values: 0
Duplicate rows: 0
Shape after duplicate check: (50000, 19)
## Cell 14
Numeric features: ['area', 'bedrooms', 'bathrooms', 'floors', 'age', 'distance', 'garage', 'parking', 'garden', 'security', 'school_nearby', 'hospital_nearby', 'shopping_mall_nearby', 'public_transport', 'crime_rate', 'population_density']
Categorical features: ['location', 'income_level']
## Cell 16
cell_16:10: UserWarning: FigureCanvasAgg is non-interactive, and thus cannot be shown
cell_16:20: UserWarning: FigureCanvasAgg is non-interactive, and thus cannot be shown
cell_16:31: UserWarning: FigureCanvasAgg is non-interactive, and thus cannot be shown
cell_16:39: UserWarning: FigureCanvasAgg is non-interactive, and thus cannot be shown
## Cell 18
X shape: (50000, 18)
y shape: (50000,)
## Cell 20
Training rows: 40000
Test rows: 10000
## Cell 22
['Linear Regression', 'Ridge Regression', 'Random Forest']
## Cell 24
Best model: Ridge Regression
## Cell 26
cell_26:19: UserWarning: FigureCanvasAgg is non-interactive, and thus cannot be shown
## Cell 29
## Cell 30
cell_30:21: UserWarning: FigureCanvasAgg is non-interactive, and thus cannot be shown
## Cell 32
## Cell 34
Best model: Ridge Regression
MAE: 15,954 price units
RMSE: 19,941 price units
R-squared: 99.81%
Main insight: area is the strongest driver, with location and income level adding market context.
## Cell 37
Final checked results
---------------------
Model: Ridge Regression
MAE: 15,954 price units
RMSE: 19,941 price units
R-squared: 99.81%
Metrics match the final report.
```
