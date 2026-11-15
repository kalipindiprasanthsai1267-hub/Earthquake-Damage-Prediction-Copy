# Earthquake Damage Prediction Using Machine Learning

## Project Overview

This project focuses on predicting the extent of building damage caused by earthquakes using Machine Learning classification algorithms.

The objective is to predict the ordinal target variable `damage_grade`, which represents three levels of building damage:

- Grade 1 – Low Damage
- Grade 2 – Medium Damage
- Grade 3 – Almost Complete Destruction

## Dataset

The project uses building-related data from the 2015 Gorkha earthquake in Nepal.

The dataset contains 260,601 building records and 38 predictor features, including geographical information, building structure, construction materials, and building characteristics.

**Dataset source:** [Original Project Dataset](https://d3ilbtxij3aepc.cloudfront.net/projects/CDS-Capstone-Projects/PRCP-1015-EquakeDamagePred.zip)

Download the dataset and place `train_values.csv` and `train_labels.csv` inside the `Data` folder before running the notebook.

## Project Workflow

1. Data loading and understanding
2. Exploratory Data Analysis (EDA)
3. Data quality checks
4. Numerical and categorical feature analysis
5. Feature preprocessing and encoding
6. Train-validation-test splitting
7. Machine Learning model development
8. Model comparison
9. XGBoost hyperparameter experiments
10. Final model evaluation
11. Challenges and solutions
12. Recommendations and conclusion

## Machine Learning Algorithms

The following models were evaluated:

- Dummy Classifier
- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- CatBoost

## Final Model – XGBoost

The original XGBoost configuration was selected based on validation performance.

### Final Test Results

| Metric | Score |
|---|---:|
| Accuracy | 73.14% |
| Macro Precision | 72.73% |
| Macro Recall | 63.45% |
| Macro F1 Score | 66.63% |
| Balanced Accuracy | 63.45% |
| Ordinal MAE | 0.2709 |
| Quadratic Weighted Kappa | 0.5811 |

## Key Findings

- Grade 2 buildings were identified more effectively than Grade 1 and Grade 3 buildings.
- Building characteristics and geographical information contributed to damage prediction.
- The model achieved 73.14% accuracy on the held-out test dataset.
- Further improvement is required in identifying low-damage and severely damaged buildings.

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- CatBoost

## Project Limitations

The model was developed using data associated with the 2015 Gorkha earthquake. Its performance may differ for other earthquakes and geographical regions.

The model is intended for predictive analysis and preliminary damage-risk screening. It is not a replacement for professional structural engineering inspections.

## Conclusion

This project demonstrates how Exploratory Data Analysis and Machine Learning can be applied to earthquake building-damage prediction.

The developed XGBoost model achieved 73.14% test accuracy. The analysis highlights the importance of safer construction, structural assessment, earthquake preparedness and further research in reducing earthquake-related damage.
