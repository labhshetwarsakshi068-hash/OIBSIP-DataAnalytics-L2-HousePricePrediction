# House Price Prediction using Linear Regression

## Project Overview
This project predicts house prices using machine learning techniques. It uses property features such as area, number of bedrooms, bathrooms, floors, year built, location, condition, and garage availability.

## Dataset
- Total records: 2,000
- Total columns in original dataset: 10
- Target variable: `Price`
- Missing values: 0
- Duplicate rows: 0

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Data Preprocessing
1. Loaded the dataset using Pandas.
2. Checked missing values and duplicate rows.
3. Removed the `Id` column because it is a record identifier.
4. Converted categorical features into numerical values using one-hot encoding.
5. Split the dataset into 80% training data and 20% testing data.

## Machine Learning Models
- Linear Regression
- Random Forest Regressor

## Model Evaluation

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | 243241.98 | 279859.73 | -0.0067 |
| Random Forest | 247761.03 | 285372.51 | -0.0468 |

## Results
Linear Regression performed slightly better than Random Forest on the test dataset. However, both models produced negative R² scores, indicating poor predictive performance.

The exploratory analysis also showed very weak relationships between the available features and house prices. The dataset may not contain sufficiently informative patterns for reliable price prediction.

## Conclusion
This project demonstrates the complete machine learning workflow, including data loading, preprocessing, model training, evaluation, visualization, and model comparison.

The current results indicate that further investigation into dataset quality and more informative features is necessary before the model can be used for reliable house price prediction.

## Project Files
- `House Price Prediction Dataset.csv` — dataset
- `model_comparison.csv` — model evaluation results
- `README.md` — project documentation
- Jupyter Notebook — preprocessing, training, evaluation, and visualizations
