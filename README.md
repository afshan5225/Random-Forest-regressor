# Random Forest Regressor Project

This project demonstrates the use of Random Forest Regressor for predicting revenue based on temperature and car prices using the CarDekho dataset.

## Terminologies
- **Bias**: Error of the training data.
- **Variance**: Error of the testing data.
- **Underfitting**: High bias, high variance.
- **Overfitting**: Low bias, high variance.

## Libraries Used
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

## Execution Methodology
1. **Data Loading**: Loaded IceCreamData.csv and cardekho_data.csv datasets.
2. **Data Preprocessing**:
   - Mapped categorical values for `Fuel_Type`, `Seller_Type`, and `Transmission` in CarDekho data.
   - Derived additional feature `no_of_years` based on the `Year` column.
3. **Modeling**:
   - Built a Random Forest Regressor to predict revenue based on temperature.
   - Used the Extra Trees Regressor to identify feature importance in predicting car selling prices.
4. **Hyperparameter Tuning**:
   - Performed RandomizedSearchCV for parameter optimization.
   - Tuned parameters such as `n_estimators`, `max_depth`, and `min_samples_split`.
5. **Evaluation**:
   - Visualized actual vs predicted values using scatter plots.
   - Checked the correlation between predicted and actual results using a heatmap.
6. **Metrics**:
   - Computed R2 score to assess model performance.
