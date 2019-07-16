# House-price-prediction-on-Amnes-dataset
Applied various regression techniques on Amnes dataset to predict house prices from 79 feature values.

## 1. Data Cleaning and preprocessing
### I. Filling missing values for various numric and categorical features.
Sterategy  : 1. Droping features with missing values more than 90%.<br>
             2. Imputing missing values with KNN in numrical columns.<br>
             3. Imputing missing values with `Most Frequent` in catogorical columns.<br>
### II. Removing Outlier.
Sterategy  : 1. Plotting scatter plot for the columns with high co-replation with 'House price'<br>
             2. Manualy deleting outlier points<br>
### III. Removing features with high co-relation.
Sterategy  : 1. Plotting heatmap for the co-relation values of top 10 columns.<br>
             2. Removing columns with high co-relations.<br>

## 2. Feature engineering
### I. Applying cos function on top 10 features (Based on co-relation with 'House price') gives much better result.

## 3. Applying LassoCV,Random forest, XGBoost and stacking on the processed data.
### 4. Removing features based on `coef_` value of Lassocv, improves result in other models.

## XGBoost gives lowest MSE of 0.02112.
