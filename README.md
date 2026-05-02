# Titanic Survival Prediction

## Project Overview
This project predicts whether a passenger survived the Titanic disaster using machine learning models. The project follows an end-to-end machine learning workflow, including data inspection, preprocessing, exploratory data analysis, feature engineering, model training, model evaluation, and model comparison.

## Dataset Overview
The dataset contains passenger information such as age, gender, passenger class, fare, family details, embarkation point, and survival status.

The target variable is `Survived`:
- `1` = Survived
- `0` = Did not survive

## Tools and Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook

## Project Workflow
1. Data Loading
2. Data Inspection
3. Data Preprocessing and Feature Engineering
4. Exploratory Data Analysis
5. Model Training and Evaluation
6. Model Comparison
7. Final Model Selection

## Feature Engineering
The following features were created to improve model performance:

- `Title`: Extracted from passenger names to capture social and demographic information.
- `FamilySize`: Created using `SibSp + Parch + 1`.
- `IsAlone`: Created to identify whether a passenger was traveling alone.
- `Fare_log`: Log transformation applied to reduce skewness in the Fare feature.

## Models Used
The following machine learning models were trained and compared:

- Logistic Regression
- Random Forest
- Tuned Random Forest
- Support Vector Machine
- XGBoost

## Best Model
XGBoost achieved the best overall performance with approximately 86% test accuracy and balanced precision, recall, and F1-score.

## Key Insights
- Female passengers had higher survival rates than male passengers.
- First-class passengers had better survival chances than second- and third-class passengers.
- Passengers traveling with family had better survival chances than passengers traveling alone.
- Higher fare was associated with better survival chances.
- Age alone was not a strong predictor due to overlap between survivors and non-survivors across age groups.

## Conclusion
This project demonstrates a complete machine learning classification workflow. XGBoost was selected as the final model because it achieved the best test performance and balanced class-wise metrics.

Although the Titanic dataset is mainly a practice dataset, this project helped build practical skills in data cleaning, EDA, feature engineering, model evaluation, and model comparison.

## How to Run
1. Clone this repository or download the files.
2. Install the required libraries:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```bash
jupyter notebook Titanic_Survival_Prediction.ipynb
```

4. Run all cells from top to bottom.
